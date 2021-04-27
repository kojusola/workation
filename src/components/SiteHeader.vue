<template>
<header class="bg-white sm:flex sm:items-center sm:justify-between">
  <div class=" px-4 py-3 flex justify-between items-center xl:w-72 xl:justify-center xl:py-5">
        <div>
          <img  class="h-8 w-auto" src="../../public/logo.png" alt= "Workation">
        </div>
      <div class="flex sm:hidden">
         <button @click="toggle" class="px-2 focus:outline-none sm:hidden">
        <svg v-if="!isOpen" class="h-6 w-5 fill-current text-gray-500  focus:text-gray-800 hover:text-gray-800" viewBox="0 0 100 80" width="40" height="40">
        <rect width="100" height="10"></rect>
        <rect y="25" width="100" height="10"></rect>
        <rect y="50" width="100" height="10"></rect>
      </svg>
      <svg class="h-6 w-6 fill-current text-gray-500" v-if="isOpen" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
         <path d="M18 6L6 18M6 6l12 12"/>
      </svg>
      </button>
      </div>
  </div>
    <nav class="sm:flex sm:items-center sm:pr-4 xl:flex-1 xl:justify-between" :class="{'hidden':!isOpen, 'block': isOpen}">
        <div class=" hidden xl:block xl:relative xl:max-w-xs xl:w-full">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3">
          <svg class="fill-current text-gray-400" xmlns="http://www.w3.org/2000/svg" width="30.24" height="30.24">
          <path d="M20.2 3.46a11.85 11.85 0 00-16.74 0 11.85 11.85 0 000 16.73c4.1 4.11 10.5 4.55 15.12 1.34.1.46.31.9.67 1.26l6.72 6.72a2.5 2.5 0 103.53-3.54l-6.71-6.72a2.5 2.5 0 00-1.26-.67c3.21-4.61 2.77-11.01-1.34-15.12zm-2.13 14.61A8.84 8.84 0 015.58 5.58a8.85 8.85 0 0112.5 12.5z"/>
        </svg>
        </div>
        <input class="block w-full bg-gray-200 text-gray-900 border-transparent focus:border-gray-300 rounded-lg pr-2 pl-11 py-2 focus:outline-none focus:bg-white focus:text-gray-900"
         type="text" placeholder="Search by keywords">
        </div>
       <div class="sm:flex sm:items-center sm:px-4">
          <div class="px-2 pb-5 sm:pb-0 sm:pt-0 pt-2 font-semibold text-gray-900 border-b border-gray-300 sm:flex sm:border-b-0 sm:text-sm sm:px-0">
          <a href="#" class="block px-3 py-1 hover:bg-gray-200 sm:px-2">List your property</a>
          <a href="#" class="block  mt-1 sm:mt-0 px-3 py-1 hover:bg-gray-200 sm:px-2 sm:ml-2">Trips</a>
          <a href="#" class="block  mt-1 sm:mt-0 px-3 py-1 hover:bg-gray-200 sm:px-2 sm:ml-2">Messages</a>
        </div>
        <div class="relative px-5 py-5 sm:py-0 sm:px-0 sm:ml-4">
          <div class="flex item-center sm:hidden">
            <img  class="h-10 w-10 object-cover rounded-full border-2 border-gray-400 sm:h-8 sm:w-8 xl:border-gray-300" src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=128&q=80" alt="">
            <span class=" ml-4 text-gray-700 font-semibold sm:hidden xl:border-gray-300">Fafemi Adeola</span>
          </div>
          <button @click="toggleDropdown" type="button" :class="[dropdownOpen ? 'sm:border-gray-700' : 'sm:border-gray-400']" class="hidden sm:block sm:h-8 sm:w-8 sm:focus:outline-none sm:focus:border-gray-700 sm:overflow-hidden sm:rounded-full sm:border-2 sm:border-gray-400 xl:border-gray-300">
             <img  class="h-full w-full object-cover sm:rounded-full" src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=128&q=80" alt="">
          </button>
          <div :class="dropdownOpen ? 'sm:block': 'sm:hidden'" class="xl:z-50">
            <button @click="dropdownOpen = false" class=" hidden sm:block sm:fixed sm:opacity-0 sm:inset-0 sm:h-full sm:w-full sm:cursor-default"></button>
          <div 
          class="mt-5 sm:rounded-lg sm:bg-white sm:absolute sm:right-0 sm:w-48 sm:mt-3 sm:py-2 sm:shadow-xl xl:z-50">
            <a href="#" class=" block text-gray-800 hover:text-black sm:text-gray-800 sm:px-4 sm:py-2 sm:hover:bg-indigo-500">Account settings</a>
            <a href="#" class="mt-3 block text-gray-800 hover:text-black sm:text-gray-800 sm:mt-0 sm:px-4 sm:py-2 sm:hover:bg-indigo-500">Support</a>
            <a href="#" class="mt-3 block text-gray-800 hover:text-black sm:text-gray-800 sm:mt-0 sm:px-4 sm:py-2 sm:hover:bg-indigo-500">Sign out</a>
          </div>

          </div>
        </div>
       </div>
      </nav>
</header>
</template>

<script>
export default {
    data (){
        return{
            isOpen:false,
            dropdownOpen:false
        }
    },
    mounted() {
      const onEscape =(e)=>{
        if (!this.dropdownOpen || e.key !== "Escape"){
          return
        }
        this.dropdownOpen = false
      }
      document.addEventListener('keydown', onEscape)
      this.$on('hook:destroyed', ()=>{
        document.removeEventListener('keydown', onEscape)
      })
    },
    methods: {
        toggle(){
            this.isOpen = !this.isOpen
        },
        toggleDropdown(){
            this.dropdownOpen = !this.dropdownOpen
        }
    }
}
</script>