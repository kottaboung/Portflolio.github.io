<script setup>
import Navbar from './components/navbar.vue'
import footbar from './components/footbar.vue'
import popup from './components/popup.vue'
import popup2 from './components/popup2.vue'
import carousel from './components/carousel.vue'
import footerrel from './components/footer.vue'
import form1 from './components/form.vue'

document.addEventListener('mousemove', (event) => {
  const image = document.getElementById('image');
  const imageRect = image.getBoundingClientRect();
  const angle = Math.atan2(event.clientY - imageRect.top - imageRect.height / 2, event.clientX - imageRect.left - imageRect.width / 2);
  const angleDegrees = angle * 10 / Math.PI;
  image.style.transform = `rotate(${angleDegrees}deg)`;
});

</script>

<template>
  
    <Navbar />
    <section id="home" class=" flex flex-col items-center my-10 )">
        <div class=" object-cover flex flex-col items-center bg-white rounded-lg gap-5 md:flex-row md:max-w-xl  dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
            <img id="image" class=" w-auto rounded-lg h-80 md:h-auto md:w-60 shadow-lg" src="https://scontent.fbkk10-1.fna.fbcdn.net/v/t1.15752-9/431972477_3727534180817564_7579294205981694598_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFv0NwseUEuFuWKHSC-g0jnMTaPV-KKiw0xNo9X4oqLDXd4KomxCVVVRuQaIoptPe9qs6vV-_Mlk9cyVNPOg-FX&_nc_ohc=JmhGNPKULloAX94g6tv&_nc_oc=AQnW2LtBt8COzmZarsut6MOo-QE3Jwg6LzyP8QxPPycT3qVyJjX0p4-vqUdwWd9M-tY&_nc_ht=scontent.fbkk10-1.fna&oh=03_AdSbvFLIAd67TNa9Eho0z3JyuLJTNZr3sm1fIvKKgjGtSA&oe=661A4298" alt="profile">
            <div class="flex flex-col justify-between px-20 py-10 md:p-4 leading-normal ">
                <h5 class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white font-sans">
                  Hello, My name is Kottaboung</h5>
                <p class="mb-3 font-normal text-gray-700 dark:text-gray-400 font-sans">
                  I am a 3rd year student from KMITL Prince Of Chumphon. I have a passion for web development in the frontend position. Right now my skills are at the beginner level. Ready to learn new things and never stop learning.</p>
                  <div class="flex flex-wrap gap-2">
                  <a href="https://raw.githubusercontent.com/kottaboung/myweb/main/pic/CV.jpg" target="_blank" 
                  class=" rounded-full bg-white hover:bg-gray-300 px-5 py-1 w-fit cursor-pointer font-bold font-mono flex gap-1">resume
                  <img class="w-6 h-6 rounded-full" src="https://www.svgrepo.com/show/445935/page-last.svg"></a>
                  <a href="https://raw.githubusercontent.com/kottaboung/myweb/main/pic/Main_trainscript.jpg" target="_blank" 
                  class=" rounded-full bg-white hover:bg-gray-300 px-5 py-1 w-fit cursor-pointer font-bold font-mono flex gap-1">Transcript
                  <img class="w-6 h-6 rounded-full" src="https://www.svgrepo.com/show/415432/copy-documents-duplicate.svg"></a>
                  <a href="https://github.com/kottaboung" target="_blank" 
                  class=" rounded-full bg-white hover:bg-gray-300 p-1 w-fit cursor-pointer font-bold font-mono">
                  <img class="w-6 h-6 rounded-full" src="https://www.svgrepo.com/show/361181/github.svg"></a>
                  <a href="https://www.facebook.com/profile.php?id=100087529516721" target="_blank" 
                  class=" rounded-full bg-white hover:bg-gray-300 p-0.5 w-fit cursor-pointer font-bold font-mono">
                  <img class="w-7 h-7 rounded-full" src="https://www.svgrepo.com/show/504313/facebook.svg"></a>
                  </div>
            </div>
          </div>
      
    </section>
    
    <section id="about" class="flex flex-col items-center my-20">
          <div class=" object-cover flex flex-col items-center bg-white rounded-lg gap-5 md:flex-row dark:border-gray-700 dark:bg-gray-800 dark:hover:bg-gray-700">
            
            <div class="flex flex-col px-10 py-5 items-center leading-normal hover:shadow-md rounded-lg gap-5">
                <h5 class="mb-2 text-2xl font-bold text-center tracking-tight text-gray-900 dark:text-white font-sans">
                  Soft Skills</h5>
                
                  <ul class="flex flex-col md:flex-row md:flex-wrap gap-3">

                    <li class="p-2 items-center flex flex-col justify-center">
                      <img class="w-16 h-16  " src="https://www.svgrepo.com/show/374447/skill.svg" alt="">
                      <p class="text-sm">Think systematically</p>
                    </li>
                    <li class="p-2 items-center flex flex-col justify-center">
                      <img class="w-16 h-16  " src="https://www.svgrepo.com/show/307996/piano-concert-skill-pianist-concert.svg" alt="">
                      <p class="text-sm">Self Learning</p>
                    </li>
                    <li class="p-2 items-center flex flex-col justify-center">
                      <img class="w-16 h-16  " src="https://www.svgrepo.com/show/421285/line-reading-text.svg" alt="">
                      <p class="text-sm">Problem solving</p>
                    </li>

                  </ul>
                  <popup />
            </div>
          
          
            
            <div class="flex flex-col px-10 py-5 items-center leading-normal hover:shadow-md rounded-lg gap-5">
                <h5 class="mb-2 text-2xl text-center font-bold tracking-tight text-gray-900 dark:text-white font-sans">
                  Hard Skills</h5>
                
                  <ul class="flex flex-col md:flex-row md:flex-wrap gap-3">

                    <li data-tooltip-target="tooltip-vue" class="p-2 items-center flex flex-col justify-center">
                      <img class="w-16 h-16  " src="https://www.svgrepo.com/show/452130/vue.svg" alt="vue">
                      <p class="text-sm">Vue Js</p>

                      <div id="tooltip-vue" role="tooltip" class="absolute z-10 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
                          4/10 point
                          <div class="tooltip-arrow" data-popper-arrow></div>
                      </div>
                    </li>
                    <li data-tooltip-target="tooltip-tailwind" class="p-2 items-center flex flex-col justify-center">
                      <img class="w-16 h-16  " src="https://www.svgrepo.com/show/374118/tailwind.svg" alt="tailwind">
                      <p class="text-sm">Tailwind CSS</p>
                      <div id="tooltip-tailwind" role="tooltip" class="absolute z-10 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
                          6/10 point
                          <div class="tooltip-arrow" data-popper-arrow></div>
                      </div>
                    </li>
                    <li data-tooltip-target="tooltip-javascript" class="p-2 items-center flex flex-col justify-center">
                      <img class="w-16 h-16  " src="https://www.svgrepo.com/show/349419/javascript.svg" alt="javascript">
                      <p class="text-sm">Javascript</p>
                      <div id="tooltip-javascript" role="tooltip" class="absolute z-10 invisible inline-block px-3 py-2 text-sm font-medium text-white transition-opacity duration-300 bg-gray-900 rounded-lg shadow-sm opacity-0 tooltip dark:bg-gray-700">
                          3/10 point
                          <div class="tooltip-arrow" data-popper-arrow></div>
                      </div>
                    </li>

                  </ul>
                  <popup2 />
            </div>
          </div>
      
    </section>


    <section id="project" class="flex flex-col items-center mb-20">
      <h1 class="text-2xl font-bold mb-5 ">My Project</h1>
      <div class="w-3/5 shadow-lg">
        <carousel />
      </div>
      
    </section>


    

    <section id="playg" class="">

    </section>

    <section id="form" class="">
      <p class=" text-2xl text-center my-5 font-bold">Contact Me !</p>
      <form1 />

    </section>
    
    <section class="mt-20">
      <footerrel />
      
    </section>
    <footbar />
  
</template>

<style scoped>
#image {
  transition: transform 0.1s ease-out;
}
</style>