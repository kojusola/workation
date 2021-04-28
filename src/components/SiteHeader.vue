<template>
<header class="bg-gray-900 sm:flex sm:items-center sm:justify-between xl:bg-white">
  <div class=" px-4 py-3 flex justify-between items-center xl:w-72 xl:justify-center xl:py-5 xl:bg-gray-900">
        <div>
          <svg class="h-8 w-auto" width="187" height="32" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M60.06 30h3.77l3.15-11.09L70.14 30h3.77l4.7-16.8h-3.47l-3.22 12.46-3.53-12.46h-2.83l-3.5 12.46-3.22-12.46h-3.48l4.7 16.8zm24.61.34A6.29 6.29 0 0091.03 24a6.29 6.29 0 00-6.36-6.34A6.27 6.27 0 0078.34 24c0 3.58 2.8 6.34 6.33 6.34zm0-3.03A3.19 3.19 0 0181.43 24a3.19 3.19 0 013.24-3.31A3.2 3.2 0 0187.94 24a3.2 3.2 0 01-3.27 3.31zm11.64-7.25V18h-3.1v12h3.1v-5.74c0-2.52 2.04-3.24 3.65-3.04v-3.46c-1.52 0-3.03.67-3.65 2.3zM112.83 30l-4.97-6.07L112.7 18h-3.7l-4.13 5.28V13.2h-3.1V30h3.1v-5.45l4.37 5.45h3.6z" fill="#fff"/>
          <path d="M120.09 30.34c2.35 0 4.4-1.25 5.42-3.12l-2.69-1.54a2.96 2.96 0 01-2.75 1.58 3.14 3.14 0 01-3.22-3.26 3.15 3.15 0 013.22-3.29c1.22 0 2.25.63 2.73 1.61l2.67-1.56a6.04 6.04 0 00-5.38-3.1 6.2 6.2 0 00-6.34 6.34 6.2 6.2 0 006.34 6.34zm16-12.34v1.42a4.78 4.78 0 00-3.92-1.76c-3.2 0-5.83 2.76-5.83 6.34s2.64 6.34 5.83 6.34c1.75 0 3.05-.68 3.91-1.76V30h3.1V18h-3.1zm-3.34 9.38a3.22 3.22 0 01-3.31-3.38 3.22 3.22 0 013.3-3.38 3.23 3.23 0 013.34 3.38 3.23 3.23 0 01-3.33 3.38zm16.1-6.4V18h-2.71v-3.36l-3.1.94V18h-2.09v2.98h2.1v4.99c0 3.24 1.46 4.51 5.8 4.03v-2.8c-1.78.09-2.71.06-2.71-1.23v-5h2.71zm3.72-4.42c1.06 0 1.92-.86 1.92-1.9 0-1.03-.87-1.92-1.92-1.92-1.03 0-1.9.9-1.9 1.92 0 1.04.87 1.9 1.9 1.9zM151.03 30h3.1V18h-3.1v12zm11.65.34a6.29 6.29 0 006.35-6.34 6.29 6.29 0 00-6.35-6.34 6.27 6.27 0 00-6.34 6.34c0 3.58 2.8 6.34 6.34 6.34zm0-3.03a3.19 3.19 0 01-3.25-3.31 3.19 3.19 0 013.25-3.31 3.2 3.2 0 013.26 3.31 3.2 3.2 0 01-3.26 3.31zm15.2-9.65c-1.6 0-2.85.6-3.57 1.68V18h-3.1v12h3.1v-6.48c0-2.09 1.13-2.98 2.64-2.98 1.4 0 2.38.84 2.38 2.48V30h3.1v-7.37c0-3.19-2-4.97-4.55-4.97z" fill="#A3BFFA"/>
          <path fill-rule="evenodd" clip-rule="evenodd" d="M42.91 11.8l-7.7-4.45V28h9v2h-44v-2h4V15.28l-3.72.93L0 14.27 21.09 9h3.12a9.55 9.55 0 00-.68 2.56l-.48 3.97 5.16-2.98V28h5V7.36l-7.7 4.44A7.5 7.5 0 0128.09 7h-4.12a7.49 7.49 0 016.65-2.97L25 .8a7.49 7.49 0 019.2 2.75A7.49 7.49 0 0143.41.8l-5.6 3.23.65-.03a7.49 7.49 0 016 3h-4.12a7.5 7.5 0 012.57 4.8zM24.21 28V18h-6v10h6zm-11-8a2 2 0 11-4 0 2 2 0 014 0z" fill="#A3BFFA"/>
          </svg>
        </div>
      <div class="flex sm:hidden">
         <button @click="toggle" class="px-2 focus:outline-none sm:hidden">
        <svg v-if="!isOpen" class="h-6 w-5 fill-current text-gray-500  focus:text-gray-800 hover:text-white" viewBox="0 0 100 80" width="40" height="40">
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
        <div class=" hidden xl:block xl:relative xl:max-w-xs xl:w-full xl:p-3">
        <div class="absolute inset-y-0 left-0 flex items-center pl-4">
          <svg class="fill-current text-gray-400" xmlns="http://www.w3.org/2000/svg" width="30.24" height="30.24">
          <path d="M20.2 3.46a11.85 11.85 0 00-16.74 0 11.85 11.85 0 000 16.73c4.1 4.11 10.5 4.55 15.12 1.34.1.46.31.9.67 1.26l6.72 6.72a2.5 2.5 0 103.53-3.54l-6.71-6.72a2.5 2.5 0 00-1.26-.67c3.21-4.61 2.77-11.01-1.34-15.12zm-2.13 14.61A8.84 8.84 0 015.58 5.58a8.85 8.85 0 0112.5 12.5z"/>
        </svg>
        </div>
        <input class="block w-full bg-gray-200 text-gray-900 border-transparent focus:border-gray-300 rounded-lg pr-2 pl-11 py-2 focus:outline-none focus:bg-white focus:text-gray-900"
         type="text" placeholder="Search by keywords">
        </div>
       <div class="sm:flex sm:items-center sm:px-4">
          <div class="px-2 pb-5 sm:pb-0 sm:pt-0 pt-2 font-semibold text-gray-900 border-b border-gray-800 sm:flex sm:border-b-0 sm:text-sm sm:px-0">
          <a href="#" class="block px-3 py-1 text-white hover:bg-gray-800 sm:px-2 xl:text-gray-900 xl:hover:bg-gray-200">List your property</a>
          <a href="#" class="block  mt-1 text-white sm:mt-0 px-3 py-1 hover:bg-gray-800 sm:px-2 sm:ml-2 xl:text-gray-900 xl:hover:bg-gray-200">Trips</a>
          <a href="#" class="block  mt-1 text-white sm:mt-0 px-3 py-1 hover:bg-gray-800 sm:px-2 sm:ml-2 xl:text-gray-900 xl:hover:bg-gray-200">Messages</a>
        </div>
        <div class="relative px-5 py-5 sm:py-0 sm:px-0 sm:ml-4">
          <div class="flex item-center sm:hidden">
            <img  class="h-10 w-10 object-cover rounded-full border-2 border-gray-400 sm:h-8 sm:w-8 xl:border-gray-300" src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=128&q=80" alt="">
            <span class=" ml-4 text-gray-200 font-semibold sm:hidden xl:border-gray-300">Fafemi Adeola</span>
          </div>
          <button @click="toggleDropdown" type="button" :class="[dropdownOpen ? 'sm:border-gray-700' : 'sm:border-gray-400']" class="hidden sm:block sm:h-8 sm:w-8 sm:focus:outline-none sm:focus:border-gray-700 sm:overflow-hidden sm:rounded-full sm:border-2 sm:border-gray-400 xl:border-gray-300">
             <img  class="h-full w-full object-cover sm:rounded-full" src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=128&q=80" alt="">
          </button>
          <div :class="dropdownOpen ? 'sm:block': 'sm:hidden'" class="xl:z-50">
            <button @click="dropdownOpen = false" class=" hidden sm:block sm:fixed sm:opacity-0 sm:inset-0 sm:h-full sm:w-full sm:cursor-default"></button>
          <div 
          class="mt-5 sm:rounded-lg sm:bg-white sm:absolute sm:right-0 sm:w-48 sm:mt-3 sm:py-2 sm:shadow-xl xl:z-50">
            <a href="#" class=" block text-gray-400 hover:text-white sm:text-gray-800 sm:px-4 sm:py-2 sm:hover:bg-indigo-500">Account settings</a>
            <a href="#" class="mt-3 block text-gray-400 hover:text-white sm:text-gray-800 sm:mt-0 sm:px-4 sm:py-2 sm:hover:bg-indigo-500">Support</a>
            <a href="#" class="mt-3 block text-gray-400 hover:text-white sm:text-gray-800 sm:mt-0 sm:px-4 sm:py-2 sm:hover:bg-indigo-500">Sign out</a>
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