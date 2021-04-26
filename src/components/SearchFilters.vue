<template>
    <section class="bg-gray-800">
      <div class="px-4 py-3 flex justify-between">
          <div class="relative max-w-xs w-full">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3">
          <svg class="fill-current text-gray-600" xmlns="http://www.w3.org/2000/svg" width="30.24" height="30.24">
          <path d="M20.2 3.46a11.85 11.85 0 00-16.74 0 11.85 11.85 0 000 16.73c4.1 4.11 10.5 4.55 15.12 1.34.1.46.31.9.67 1.26l6.72 6.72a2.5 2.5 0 103.53-3.54l-6.71-6.72a2.5 2.5 0 00-1.26-.67c3.21-4.61 2.77-11.01-1.34-15.12zm-2.13 14.61A8.84 8.84 0 015.58 5.58a8.85 8.85 0 0112.5 12.5z"/>
        </svg>
        </div>
        <input class="block w-full bg-gray-900 text-white rounded-lg pr-2 pl-11 py-2 focus:outline-none focus:bg-white focus:text-gray-900"
         type="text" placeholder="Search by keywords">
      </div>
      <button @click="toggle"
       class=" ml-4 flex items-center bg-gray-700 text-white font-medium focus:outline-none focus:shadow-outline focus:text-gray-900 rounded-lg pr-3 pl-2"
       :class="{'bg-gray-600':isOpen, 'hover:bg-gray-600 shadow':!isOpen}">
        <svg width="28" height="28" class="fill-current text-gray-500" xmlns="http://www.w3.org/2000/svg">
          <path d="M17 19a1 1 0 010 2h-6a1 1 0 010-2h6zm4-6a1 1 0 010 2H7a1 1 0 010-2h14zm3-6a1 1 0 010 2H4a1 1 0 110-2h20z"/>
        </svg>
        <span class="ml-1 text-white">Filters</span>
      </button>
      </div>
      <form v-show="isOpen">
          <div class="lg:flex">
        <fieldset class="px-4 py-4 border-t border-gray-900 sm:flex lg:w-1/3 lg:flex lg:flex-wrap">
              <div class="flex sm:w-1/2 lg:w-full">
                  <label class="w-1/2 pr-2 lg:w-1/2">
                      <span class="block text-sm font-semibold text-gray-500">Bedrooms</span>
                      <select class="mt-1 border-transparent leading-snug rounded-lg bg-gray-700 form-select w-full text-white shadow focus:bg-gray-600 focus:shadow-none">
                          <option>4</option>
                          <option>3</option>
                      </select>
                  </label>
                  <label class="w-1/2 pl-2 lg:w-1/2">
                      <span class="block text-sm font-semibold text-gray-500">Bathrooms</span>
                      <select class="mt-1 border-transparent leading-snug rounded-lg bg-gray-700 w-full text-white shadow focus:bg-gray-600 focus:shadow-none">
                          <option>2</option>
                          <option>1</option>
                      </select>
                  </label>
              </div>
              <div class="mt-6 sm:w-1/2 sm:mt-0 sm:pl-3 lg:w-full lg:pl-0 lg:mt-2">
                  <label>
                      <span class="block text-sm font-semibold text-gray-500">Price Range</span>
                      <select class=" mt-1 w-full border-transparent leading-snug rounded-lg bg-gray-700 form-select text-white shadow focus:bg-gray-600 focus:shadow-none">
                          <option>Up to $2000/wk</option>
                      </select>
                  </label>
              </div>
          </fieldset>
          <fieldset class="px-4 py-4 border-t border-gray-900 lg:w-1/3 lg:border-l">
              <span class="block text-sm font-semibold text-gray-500">Property Type</span>
              <div class="sm:flex sm:-mx-2 lg:block lg:mx-0">
              <label class=" mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-full lg:px-0">
                  <input class="form-radio bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="radio" name="propertyType" value="house">
                  <span class="ml-2 text-white">House</span> 
              </label>
              <label class=" mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-full lg:px-0">
                  <input class="form-radio bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="radio" name="propertyType" value="apartment">
                  <span class="ml-2 text-white">Apartment</span>
              </label >
              <label class="mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-full lg:px-0">
                  <input class="form-radio bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="radio" name="propertyType" value="loft">
                  <span class="ml-2 text-white">loft</span>
              </label>
              <label class=" mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-full lg:px-0">
                  <input class="form-radio bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="radio" name="propertyType" value="townhouse">
                  <span class="ml-2 text-white">Townhouse</span>
              </label>
              </div>
          </fieldset>
          <fieldset class="px-4 py-4 border-t border-gray-900 lg:w-1/3 lg:border-l">
              <span class="mt-3 sm:mt-0 block text-sm font-semibold text-gray-500 checked:bg-indigo-500">Amenities</span>
            <div class="sm:flex sm:-mx-2 sm:flex-wrap">
             <label class="mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-1/2">
                  <input class="form-checkbox bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="checkbox" name="balcony">
                  <span class="ml-2 text-white">Balcony</span>
              </label>
              <label class=" mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-1/2">
                  <input class="form-checkbox bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="checkbox" name="airConditioning">
                    <span class="ml-2 text-white">Air conditioning</span>
              </label >
              <label class=" mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-1/2">
                  <input class="form-checkbox bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="checkbox" name="pool">
                  <span class="ml-2 text-white">Pool</span>
              </label>
              <label class=" mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-1/2">
                  <input class="form-checkbox bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="checkbox" name="beach">
                  <span class="ml-2 text-white">Beach</span>
              </label>
              <label class=" mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-1/2">
                  <input class="form-checkbox bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="checkbox" name="petFriendly">
                  <span class="ml-2 text-white">Pet Friendly</span>
              </label>
              <label class=" mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-1/2">
                  <input class="form-checkbox bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="checkbox" name="kidFriendly">
                  <span class="ml-2 text-white">Kid Friendly</span>
              </label>
              <label class=" mt-3 sm:w-1/4 sm:px-2 flex items-center lg:w-1/2">
                  <input class="form-checkbox bg-gray-900 border-transparent checked:bg-indigo-500 bg-gray-700" type="checkbox" name="parking">
                  <span class="ml-2 text-white">Parking</span>
              </label>
              </div>
          </fieldset>
          </div>
          <div class="bg-gray-900 px-4 py-4 sm:text-right">
              <button class="block w-full bg-indigo-500 hover:bg-indigo-400 font-semibold text-white px-4 py-2 rounded-lg sm:w-auto sm:inline-block">Update Results</button>
          </div>
      </form>
    </section>
</template>

<script>
export default {
     data (){
        return{
            isOpen:true
        }
    },
    methods: {
        toggle(){
            this.isOpen = !this.isOpen
        }
    }
}
</script>

<style scoped>

</style>