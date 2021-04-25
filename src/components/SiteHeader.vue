<template>
<header class="bg-white sm:flex sm:items-center sm:justify-between">
  <div class=" px-4 py-3 flex justify-between items-center">
        <div>
          <img  class="h-8 w-auto" src="../../public/logo.png" alt= "Workation">
        </div>
      <div class="flex">
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
        <nav class="sm-block" :class="{'hidden':!isOpen, 'block': isOpen}">
        <div class="px-2 pb-5 sm:pb-0 sm:pt-0 pt-2 font-semibold border-b border-gray-300 sm:flex sm:border-b-0 sm:text-sm">
          <a href="#" class="block px-3 py-1 hover:bg-gray-200 sm:px-2">List your property</a>
          <a href="#" class="block  mt-1 sm:mt-0 px-3 py-1 hover:bg-gray-200 sm:px-2 sm:ml-2">Trips</a>
          <a href="#" class="block  mt-1 sm:mt-0 px-3 py-1 hover:bg-gray-200 sm:px-2 sm:ml-2">Messages</a>
        </div>
        <div class="px-5 py-5 sm:hidden">
          <div class="flex item-center">
            <img  class="h-10 w-10 object-cover rounded-full border-2 border-gray-400" src="https://images.unsplash.com/photo-1487412720507-e7ab37603c6f?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=128&q=80" alt="">
            <span class=" ml-4 text-gray-700 font-semibold">Fafemi Adeola</span>
          </div>
          <div class="mt-5">
            <a href="#" class=" block text-gray-800 hover:text-black">Account settings</a>
            <a href="#" class="mt-3 block text-gray-800 hover:text-black">Support</a>
            <a href="#" class="mt-3 block text-gray-800 hover:text-black">Sign out</a>
          </div>
        </div>
      </nav>
</header>
</template>

<script>
export default {
    data (){
        return{
            isOpen:false
        }
    },
    methods: {
        toggle(){
            this.isOpen = !this.isOpen
        }
    }
}
</script>