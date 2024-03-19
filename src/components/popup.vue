<template>
    <div id="pop" class="flex flex-col items-center">
       
        <div v-if="showGrid" id="gridContainer" class="grid-container">
        
        <ul class="flex flex-col md:flex-row md:flex-wrap gap-3 grid-item">

            <li class="p-2 items-center flex flex-col justify-center">
            <img class="w-16 h-16  " src="https://www.svgrepo.com/show/265454/teamwork-team.svg" alt="">
            <p class="text-sm">Team Collaboration</p>
            </li>
            

        </ul>
        </div>
        <div class="w-fit">
        <button @click="toggleGrid" class=" rounded-full px-3 py-2 hover:shadow-md hover:bg-gray-100 my-5">
          <img  class="w-8 h-8 ratateDegree" :class="{'rotate-180' : isRotated }" src="https://www.svgrepo.com/show/522521/down-2.svg"  id="myImage" >
        </button></div>
    </div>
</template>

<script>
export default {
name:"popup",
  data() {
    return {
      showGrid: false,
      isRotated: false,
    };
  },
  methods: {
    toggleGrid() {
      this.showGrid = !this.showGrid;
      this.isRotated = !this.isRotated;
    }
  }
}
</script>

