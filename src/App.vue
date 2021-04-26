<template>
  <div id="app" class="min-h-screen bg-gray-200 antialiased">
    <SiteHeader/>
    <SearchFilters/>
    <main class=" py-6">
      <div class="px-4">
        <h3 class="text-gray-900 text-xl">Los Angeles</h3>
        <p class="text-gray-600">Live like the stars in these luxurious Southern California estates</p>
      </div>
     <div class="sm:flex  sm:overflow-x-auto sm:pl-1 sm:pr-6">
      <div class="mt-5 sm:max-w-xs sm:w-full sm:flex-shrink-0 px-4">
        <div class="sm:max-w-xs sm:w-full sm:flex-shrink-0">
          <div class="relative pb-5/6">
             <img class="absolute inset-0 rounded-lg shadow-md h-full object-cover" src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=750&q=80" alt="">
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
       <div class="mt-5 px-4 sm:max-w-xs sm:w-full sm:flex-shrink-0 sm:px-2">
        <div class="sm:max-w-xs sm:w-full sm:flex-shrink-0 ">
          <div class="relative pb-5/6">
             <img class="absolute inset-0 rounded-lg shadow-md h-full object-cover" src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=750&q=80" alt="">
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
       <div class="mt-5 px-4 sm:max-w-xs sm:w-full sm:flex-shrink-0 sm:px-2">
        <div class="sm:max-w-xs sm:w-full sm:flex-shrink-0">
          <div class="relative pb-5/6">
             <img class="absolute inset-0 rounded-lg shadow-md h-full object-cover" src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=750&q=80" alt="">
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
       <div class="mt-5 px-4 sm:max-w-xs sm:w-full sm:flex-shrink-0 sm:px-2">
        <div class="sm:max-w-xs sm:w-full sm:flex-shrink-0 ">
          <div class="relative pb-5/6">
             <img class="absolute inset-0 rounded-lg shadow-md h-full object-cover" src="https://images.unsplash.com/photo-1512917774080-9991f1c4c750?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=750&q=80" alt="">
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
     </div>
    </main>

  </div>
</template>

<script>

import SiteHeader from "./components/SiteHeader"
import SearchFilters from "./components/SearchFilters"
export default {
  name: 'App',
  components: {
   SiteHeader,
   SearchFilters
  }
}
</script>

<style>

</style>
