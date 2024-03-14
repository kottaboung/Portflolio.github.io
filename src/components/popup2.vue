<template>
    <div id="pop" class="flex flex-col ">
        <button @click="toggleGrid" class=" rounded-full px-3 py-2 hover:shadow-md hover:bg-gray-100 my-5">See More</button>
        <div v-if="showGrid" id="gridContainer" class="grid-container">
        
        <ul class="flex flex-col md:grid md:grid-cols-3 md:grid-flow-row  gap-3 grid-item">

            <li data-tooltip-target="tooltip-python" class="p-2 items-center flex flex-col justify-center">
            <img class="w-16 h-16  " src="https://www.svgrepo.com/show/452091/python.svg" alt="">
            <p class="text-sm">Python</p>

              <div id="tooltip-python" role="tooltip" class="absolute z-50 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
                  5/10 point
                  <div class="tooltip-arrow" data-popper-arrow></div>
              </div>

            </li>
            <li data-tooltip-target="tooltip-c" class="p-2 items-center flex flex-col justify-center">
            <img class="w-16 h-16  " src="https://www.svgrepo.com/show/508906/cplusplus.svg" alt="">
            <p class="text-sm">C++</p>
              <div id="tooltip-c" role="tooltip" class="absolute z-50 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
                  6/10 point
                  <div class="tooltip-arrow" data-popper-arrow></div>
              </div>

            </li>
            <li data-tooltip-target="tooltip-bootstrap" class="p-2 items-center flex flex-col justify-center">
            <img class="w-16 h-16  " src="https://www.svgrepo.com/show/353498/bootstrap.svg" alt="">
            <p class="text-sm">Bootstrap</p>
              <div id="tooltip-bootstrap" role="tooltip" class="absolute z-50 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
                  5/10 point
                  <div class="tooltip-arrow" data-popper-arrow></div>
              </div>
            </li>
            <li data-tooltip-target="tooltip-html" class="p-2 items-center flex flex-col justify-center">
            <img class="w-16 h-16  " src="https://www.svgrepo.com/show/452228/html-5.svg" alt="">
            <p class="text-sm">HTML</p>
              <div id="tooltip-html" role="tooltip" class="absolute z-50 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
                  9/10 point
                  <div class="tooltip-arrow" data-popper-arrow></div>
              </div>
            </li>
            <li data-tooltip-target="tooltip-css" class="p-2 items-center flex flex-col justify-center">
            <img class="w-16 h-16  " src="https://www.svgrepo.com/show/452185/css-3.svg" alt="">
            <p class="text-sm">CSS</p>
              <div id="tooltip-css" role="tooltip" class="absolute z-50 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
                  8/10 point
                  <div class="tooltip-arrow" data-popper-arrow></div>
              </div>
            </li>
            <li data-tooltip-target="tooltip-php" class="p-2 items-center flex flex-col justify-center">
            <img class="w-16 h-16  " src="https://www.svgrepo.com/show/349474/php.svg" alt="">
            <p class="text-sm">PHP</p>
              <div id="tooltip-php" role="tooltip" class="absolute z-50 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
                  5/10 point
                  <div class="tooltip-arrow" data-popper-arrow></div>
              </div>
            </li>


        </ul>
        </div>
    </div>
</template>

<script>
export default {
name:"popup2",
  data() {
    return {
      showGrid: false,
      
    };
  },
  methods: {
    toggleGrid() {
      this.showGrid = !this.showGrid;
      
    }
  }
}
</script>

