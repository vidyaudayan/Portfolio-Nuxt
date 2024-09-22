<template>
  <section id="about" class="flex flex-col md:flex-row items-center bg-cyan-100 py-10">
    <div class="md:w-1/2 mb-6 ml-4 mr-4 md:mb-0 ">
      <img
        src="assets/images/about.avif" 
        alt="About Me"
        class="w-96  rounded-lg shadow-lg"
      />
     
    </div>
    <div class="md:w-1/2 md:pl-8 mr-4">
      <h2 class="text-3xl font-bold mb-4 ml-2">About Me</h2>
      <p class="text-lg mb-6 ml-2">
       Enthusiastic and adaptable full-stack developer passionate about learning and working in web development technologies. Seeking to leverage diverse technical skills and programming expertise in a dynamic Full Stack Developer role. Eager to contribute innovative solutions to complex software development challenges while continuously expanding knowledge of cutting-edge technologies. Committed to delivering high-quality, scalable applications that drive business success and user satisfaction.
      </p>
      <a 
        href= "/resume.pdf" 
        target="_blank" 
        class="bg-black m-1 text-white py-2 px-4 rounded hover:bg-white hover:text-black transition duration-300"
      >
    
        View Resume
      </a>
    </div>
  </section>
</template>

<script>
export default {
  name: 'AboutMe',

  }
</script>


<style scoped>
  .pdf-container {
    height: 500px;
  }
</style>