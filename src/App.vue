<template>
  <div id="app" class="min-h-screen bg-gray-200 antialiased">
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
      <button class="flex items-center text-white font-medium bg-gray-700 hover:bg-gray-600 focus:outline-none focus:shadow-outline focus:text-gray-900 rounded-lg shadow pr-3 pl-2">
        <svg width="28" height="28" class="fill-current text-gray-500" xmlns="http://www.w3.org/2000/svg">
          <path d="M17 19a1 1 0 010 2h-6a1 1 0 010-2h6zm4-6a1 1 0 010 2H7a1 1 0 010-2h14zm3-6a1 1 0 010 2H4a1 1 0 110-2h20z" fill="#212121" fill-rule="nonzero"/>
        </svg>
        <span class="ml-1">Filters</span>
      </button>
    </section>
    <main class="px-4 py-6">
      <h3 class="text-gray-900 text-xl">Los Angeles</h3>
      <p class="text-gray-600">Live like the stars in these luxurious Southern California estates</p>
      <div class="mt-5">
        <div>
          <div>
             <img class="rounded-lg shadow-md h-64" src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=750&q=80" alt="">
          </div>
          <div class="relative px-4 -mt-16 ">
            <div class="bg-white rounded-lg px-4 py-4 shadow-lg">
            <div class="flex ">
              <span class="inline-block font-semibold rounded-full px-1 py-1 leading-none tracking-wide text-xs bg-blue-100 text-blue-400">
                PLUS
                </span>
              <div class="ml-2 text-xs text-gray-600 font-semibold uppercase tracking-wide">
                3 beds &bull; baths
              </div>
            </div>
            <h4 class="mt-1 text-gray-900 font-semibold text-lg">Modern Home in city center</h4>
            <div class="mt-1">
              <span class="text-gray-900 ">1,400</span>
              <span class="ml-1 text-sm text-gray-600">/wk</span>
            </div>
            <div class="flex  items-center text-sm text-gray-600">
              <svg class="h-3 w-3  fill-current text-blue-400" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 329.94 329.94">
                 <path d="M329.2 126.67a15 15 0 00-12.1-10.21l-95.82-13.93-42.86-86.83a15 15 0 00-26.9 0l-42.85 86.83-95.82 13.93a15 15 0 00-8.32 25.58l69.34 67.58-16.37 95.45a15 15 0 0021.76 15.81l85.71-45.06 85.71 45.06a15 15 0 0021.62-16.63l-16.23-94.63 69.34-67.58a15 15 0 003.8-15.37z"/>
              </svg>
              <svg class="h-3 w-3 ml-1 fill-current text-blue-400" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 329.94 329.94">
                 <path d="M329.2 126.67a15 15 0 00-12.1-10.21l-95.82-13.93-42.86-86.83a15 15 0 00-26.9 0l-42.85 86.83-95.82 13.93a15 15 0 00-8.32 25.58l69.34 67.58-16.37 95.45a15 15 0 0021.76 15.81l85.71-45.06 85.71 45.06a15 15 0 0021.62-16.63l-16.23-94.63 69.34-67.58a15 15 0 003.8-15.37z"/>
              </svg>
              <svg class="h-3 w-3 ml-1 fill-current text-blue-400" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 329.94 329.94">
                 <path d="M329.2 126.67a15 15 0 00-12.1-10.21l-95.82-13.93-42.86-86.83a15 15 0 00-26.9 0l-42.85 86.83-95.82 13.93a15 15 0 00-8.32 25.58l69.34 67.58-16.37 95.45a15 15 0 0021.76 15.81l85.71-45.06 85.71 45.06a15 15 0 0021.62-16.63l-16.23-94.63 69.34-67.58a15 15 0 003.8-15.37z"/>
              </svg>
              <svg class="h-3 w-3 ml-1 fill-current text-blue-400" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 329.94 329.94">
                 <path d="M329.2 126.67a15 15 0 00-12.1-10.21l-95.82-13.93-42.86-86.83a15 15 0 00-26.9 0l-42.85 86.83-95.82 13.93a15 15 0 00-8.32 25.58l69.34 67.58-16.37 95.45a15 15 0 0021.76 15.81l85.71-45.06 85.71 45.06a15 15 0 0021.62-16.63l-16.23-94.63 69.34-67.58a15 15 0 003.8-15.37z"/>
              </svg>
              <svg class="h-3 w-3 mx-1 fill-current text-blue-400" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 329.94 329.94">
                 <path d="M329.2 126.67a15 15 0 00-12.1-10.21l-95.82-13.93-42.86-86.83a15 15 0 00-26.9 0l-42.85 86.83-95.82 13.93a15 15 0 00-8.32 25.58l69.34 67.58-16.37 95.45a15 15 0 0021.76 15.81l85.71-45.06 85.71 45.06a15 15 0 0021.62-16.63l-16.23-94.63 69.34-67.58a15 15 0 003.8-15.37z"/>
              </svg>
              34 reviews
            </div>
          </div>
          </div>
        </div>
      </div>
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
