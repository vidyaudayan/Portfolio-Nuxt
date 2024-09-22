

{/*<template>
  <header class="bg-white shadow-md fixed w-full top-0 z-50">
    <div class="container mx-auto flex items-center justify-between p-4">
      <!-- Logo -->
      <div class="text-3xl  font-bold">
        <a href="#home">Portfolio</a>
      </div>

      <!-- Desktop Navigation Links -->
      <nav class="hidden md:flex space-x-6 text-lg">
        <a href="#about" class="hover:text-cyan-500 font-semibold">About Me</a>
        <a href="#skills" class="hover:text-cyan-500 font-semibold">Skills</a>
        <a href="#projects" class="hover:text-cyan-500 font-semibold">Projects</a>
        <a href="#contact" class="hover:text-cyan-500 font-semibold">Contact </a>
      </nav>

      <!-- Mobile Menu Icon -->
      <div class="md:hidden">
        <button @click="toggleMenu">
          <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-black" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"/>
          </svg>
        </button>
      </div>

      <!-- Mobile Navigation Menu -->
      <nav v-if="isMenuOpen" class="fixed inset-0 bg-transparent flex flex-col items-center mt-14 md:hidden">
        <a href="#about" class="py-2 text-white text-xl hover:text-blue-500" @click="toggleMenu">About Me</a>
        <a href="#skills" class="py-2 text-xl text-white hover:text-blue-500" @click="toggleMenu">Skills</a>
        <a href="#projects" class="py-2 text-xl text-white hover:text-blue-500" @click="toggleMenu">Projects</a>
        <a href="#contact" class="py-2 text-xl text-white hover:text-blue-500" @click="toggleMenu">Contact Info</a>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    },
  },
};
</script>

<style scoped>
/* Add any additional styles if necessary */
</style>*/}