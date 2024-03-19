<template>
 
    <div class="py-6 mx-10 flex justify-between border-b mb-2">
      <div class=" cursor-pointer rounded-full hover:shadow-sm py-1 px-2">
       <p class="text-2xl font-bold font-mono">PortFlolio</p>
      </div>
      <div>
       <ul class="md:flex gap-5 hidden ">
           <li class="px-5 rounded-full py-1 hover:bg-gray-50 cursor-pointer">
               <a href="#home">Home</a>
           </li>
           <li class="px-5 rounded-full py-1 hover:bg-gray-50 cursor-pointer">
               <a href="#about">About</a>
           </li>
           <li class="px-5 rounded-full py-1 hover:bg-gray-50 cursor-pointer">
               <a href="#project">Project</a>
           </li>
           <li class="px-5 rounded-full py-1 hover:bg-gray-50 cursor-pointer">
               <a href="#contact">Contact</a>
           </li>
       </ul>
       
      </div> 
      <div>
       <ul class="flex gap-5">
           
           <div class=" flex rounded-full cursor-pointer hover:bg-gray-50 border hover:shadow-md">
                <button id="dropdownUsersButton" data-dropdown-toggle="dropdownUsers" data-dropdown-placement="bottom" class=" bg-gray-100 hover:bg-gray-300 focus:ring-4 focus:outline-none focus:ring-gray-100 font-medium rounded-full text-sm px-5 py-2.5 text-center inline-flex items-center " type="button">ME<svg class="w-2.5 h-2.5 ms-3" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 10 6">
                <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="m1 1 4 4 4-4"/>
                </svg>
                </button>

                <!-- Dropdown menu -->
                <div id="dropdownUsers" class="z-10 hidden bg-white rounded-lg shadow w-60 dark:bg-gray-700">
                <ul class="h-auto py-2 overflow-y-auto text-gray-700 dark:text-gray-200" aria-labelledby="dropdownUsersButton">
                    
                    <li>
                    <a href="#" class="flex items-center px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">
                        <img class="w-10 h-10 me-2 rounded-full" src="https://github.com/kottaboung/myweb/blob/main/pic/a.JPG?raw=true" alt="Jese image">
                        Kottaboung Nanvong<br>
                        64200002@kmitl.ac.th<br>
                        
                    </a>
                    </li>
                    <li class=" px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">
                        <a><p class=" text-center">Tel : 098-016-9099</p></a>
                    </li>
                </ul>
                
                </div>

            </div>
       </ul>
      </div> 
    </div>
   
   
   </template>
   
   
   <script>
   export default {
   name:"Navbar"
   }
   </script>
   
   <style>
   
   </style>