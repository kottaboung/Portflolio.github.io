<template>
  <div class=" w-screen h-fit flex justify-center gap-10">
    <div class=" hidden md:grid align-middle items-center"> 
      <img class=" h-60" src="https://sites.psu.edu/curtmoore34/wp-content/uploads/sites/40170/2016/04/contactme.png">
      
    </div>
    <div class=" my-5">
      <form action="https://formspree.io/f/mqkrdbvl" method="POST">
        <div class="mt-8">
          <spna class=" uppercase text-sm text-gray-600 font-bold">Name</spna>
          <input name="name" class=" w-full bg-gray-200 text-gray-900 mt-2 p-3 rounded-lg focus:outline-none focus:shadow-outline"
          type="text" placeholder="Enter Your Name" required>
        </div>
        <div class="mt-8">
          <spna class=" uppercase text-sm text-gray-600 font-bold">Email</spna>
          <input name="email" class=" w-full bg-gray-200 text-gray-900 mt-2 p-3 rounded-lg focus:outline-none focus:shadow-outline"
          type="text" placeholder="Enter Your Email" required>
        </div>
        <div class="mt-8">
          <span class="uppercase text-sm text-gray-600 font-bold">Message</span>
          <textarea name="1message" class="w-full h-32 bg-gray-200 text-gray-900 mt-2 p-3 rounded-lg focus:outline-none focus:shadow-outline" required></textarea>
        </div>
        <button type=" submit"
          class="mt-8 uppercase text-sm font-bold tracking-wide bg-indigo-500 text-gray-100 p-3 
          rounded-lg w-full focus:outline-none focus:shadow-outline hover:bg-indigo-600 hover:shadow-md">
          Send Message
          </button>
      </form>
    </div>
  </div>


        
</template>

<script>

export default {
name:"form1",
}

</script>

<style>

</style>