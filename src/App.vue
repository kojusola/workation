<template>
  <div id="app" class="bg-gray-200 antialiased">
    <header class="bg-white px-4 py-3 flex justify-between items-center">
      <div>
        <img  class="h-8 w-auto" src="../public/logo.png" alt= "Workation">
      </div>
      <div class="flex">
         <button>
        <svg  class="h-6 w-5 fill-current text-gray-500" viewBox="0 0 100 80" width="40" height="40">
        <rect width="100" height="10"></rect>
        <rect y="25" width="100" height="10"></rect>
        <rect y="50" width="100" height="10"></rect>
      </svg>
      </button>
      </div>
    </header>
    <section class="bg-gray-800 px-4 py-3 flex justify-between">
      <div class="relative">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3">
          <svg class="fill-current text-gray-600" xmlns="http://www.w3.org/2000/svg" width="30.24" height="30.24">
          <path d="M20.2 3.46a11.85 11.85 0 00-16.74 0 11.85 11.85 0 000 16.73c4.1 4.11 10.5 4.55 15.12 1.34.1.46.31.9.67 1.26l6.72 6.72a2.5 2.5 0 103.53-3.54l-6.71-6.72a2.5 2.5 0 00-1.26-.67c3.21-4.61 2.77-11.01-1.34-15.12zm-2.13 14.61A8.84 8.84 0 015.58 5.58a8.85 8.85 0 0112.5 12.5z"/>
        </svg>
        </div>
        <input class="bg-gray-900 text-white rounded-lg pr-2 pl-11 py-2 focus:outline-none focus:bg-white focus:text-gray-900"
         type="text" placeholder="Search by keywords">
      </div>
      <button class="flex items-center text-white font-medium bg-gray-700 hover:bg-gray-600 rounded-lg shadow pr-3 pl-2">
        <svg width="28" height="28" class="fill-current text-gray-500" xmlns="http://www.w3.org/2000/svg">
          <path d="M17 19a1 1 0 010 2h-6a1 1 0 010-2h6zm4-6a1 1 0 010 2H7a1 1 0 010-2h14zm3-6a1 1 0 010 2H4a1 1 0 110-2h20z" fill="#212121" fill-rule="nonzero"/>
        </svg>
        <span class="ml-1">Filters</span>
      </button>
    </section>
    <main class="">
      <h3>Los Angeles</h3>
      <p>Live like the stars in these luxurious Southern California estates</p>
    </main>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
   
  }
}
</script>

<style>

</style>
