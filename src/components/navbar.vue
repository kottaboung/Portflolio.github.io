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
       </ul>
       
      </div> 
      <div>
       <ul class="flex gap-5">
           
           <div class=" flex rounded-full cursor-pointer hover:bg-gray-50 border hover:shadow-md">
               
               <img class="h-10 w-10 rounded-full p-1" src="https://github.com/kottaboung/myweb/blob/main/pic/a.JPG?raw=true" alt="logo">
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