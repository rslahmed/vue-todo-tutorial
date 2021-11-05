<template>
  <div
      class="h-screen w-screen bg-gradient-to-tr from-blue-400 to-red-300 flex flex-col items-center justify-center px-4 space-y-3">
    <!-- Logo -->
    <div class="text-white">
      <svg xmlns="http://www.w3.org/2000/svg" class="h-12 w-12" fill="none" viewBox="0 0 24 24" stroke="currentColor">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-6 9l2 2 4-4"/>
      </svg>
    </div>
    <!-- Logo end-->

    <!-- List box -->
    <div class="bg-white p-8 w-full max-w-xl rounded">
      <!-- Add task -->
      <form class="flex">
        <input
            type="text"
            class="block w-full border border-gray-300 focus:border-gray-400 focus:outline-none rounded-l-md px-4 py-1.5"
            placeholder="Add task to your list"/>
        <button
            type="submit"
            class="border border-gray-300 border-l-0 rounded-r-md px-6 py-1 bg-indigo-500 hover:bg-indigo-600 text-white">
          Add
        </button>
      </form>
      <!-- Add task end-->

      <!-- search -->
      <div class="flex items-center justify-between mt-4">
        <h3 class="text-gray-600">Your tasks:</h3>
        <div class="flex items-center h-8">
          <!-- Search -->
          <button>
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-gray-600" fill="none" viewBox="0 0 24 24"
                 stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/>
            </svg>
          </button>

          <!-- After clicking search icon -->
          <div class="relative">
            <input type="text"
                   class="w-56 rounded-md block border border-gray-300 text-sm px-7 py-1"
                   placeholder="search your task"/>
            <span class="absolute left-1.5 top-2 text-gray-400">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4 " fill="none" viewBox="0 0 24 24"
                   stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/>
              </svg>
            </span>
            <button class="absolute right-1.5 top-2 text-gray-400 hover:text-gray-700">
              <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24"
                   stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"/>
              </svg>
            </button>
          </div>
          <!-- Search end -->
        </div>
      </div>
      <!-- search end -->

      <!-- Tasks List -->
      <div class="mt-5 space-y-1">
        <div class="px-3 py-1.5 bg-indigo-50 hover:bg-indigo-100 rounded flex items-center group">
          <input type="checkbox" class="w-4 h-4 rounded text-indigo-500 cursor-pointer"/>
          <span class="text-gray-800 ml-3">I am a task</span>
          <button class="text-red-500 ml-auto group-hover:block hidden hover:text-red-600">
            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" fill="none" viewBox="0 0 24 24"
                 stroke="currentColor">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M19 7l-.867 12.142A2 2 0 0116.138 21H7.862a2 2 0 01-1.995-1.858L5 7m5 4v6m4-6v6m1-10V4a1 1 0 00-1-1h-4a1 1 0 00-1 1v3M4 7h16"/>
            </svg>
          </button>
        </div>
        <div class="text-gray-600 text-center mt-8">
          You have no tasks :)
        </div>
      </div>
      <!-- Tasks List end -->

      <!-- Clear all -->
      <div class="mt-4">
        <button class="px-6 py-1.5 text-white bg-indigo-500 hover:bg-indigo-600 rounded text-sm">
          Clear all
        </button>
      </div>
      <!-- Clear all end -->

    </div>
    <!-- List box end -->
  </div>
</template>

<script>
export default {
  
}
</script>