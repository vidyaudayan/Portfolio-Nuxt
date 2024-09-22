<template>
  <Header />

  <div
    class="relative w-full h-screen bg-cover bg-center bg-[url('/assets/images/background3.avif')]"
  >
    <!-- Left Side Content -->
    <div class="absolute top-1/2 left-10 transform -translate-y-1/2 text-white">
      <h1 class="text-5xl font-bold">Hello, It's me</h1>
      <h2 class="text-6xl font-extrabold mt-2">Vidyamol Udayan</h2>

      <!-- Text Animation -->
      <p class="text-3xl mt-4 h-10 overflow-hidden">
        <span
          class="block text-cyan-500 animate-slide-upp"
          v-if="isVisible"
          v-text="currentRole"
        ></span>
      </p>

      <!-- Expertise Description -->
      <p class="text-lg mt-4 max-w-md">
        Expertise in creating interactive user interfaces and robust server-side
        applications.
      </p>

      <!-- Social Media Icons -->
      <div class="flex mt-6 space-x-4">
        <a
          href="https://github.com/vidyaudayan"
          target="_blank"
          class="text-white hover:text-cyan-400"
        >
          <font-awesome-icon :icon="['fab', 'github']" class="text-4xl" />
       
        </a>

        <a
          href="https://linkedin.com/in/vidyamoludayan"
          target="_blank"
          class="text-white hover:text-cyan-400"
        >
          <font-awesome-icon :icon="['fab', 'linkedin']" class="text-4xl" />
        </a>
        <a
          href="https://google.co.in" target="_blank"
          class="text-white hover:text-cyan-400"
        >
          <font-awesome-icon :icon="['fas', 'envelope']" class="text-4xl" />
        </a>
      </div>
    </div>

    <!-- Right Side Profile Image -->
   
  </div>
</template>

<script>
export default {
  data() {
    return {
      roles: ['Back-end Developer', 'Front-end Developer', 'Full Stack Web Developer'],
      currentIndex: 0,
      currentRole: 'Back-end Developer',
      isVisible: true, // Visibility control for text transition
    };
  },
  mounted() {
    this.cycleRoles();
  },
  methods: {
    cycleRoles() {
      setInterval(() => {
        this.isVisible = false; // Hide text momentarily
        setTimeout(() => {
          this.currentIndex = (this.currentIndex + 1) % this.roles.length;
          this.currentRole = this.roles[this.currentIndex];
          this.isVisible = true; // Show the updated role
        }, 300); // Brief delay before showing new role
      }, 3000); // Change role every 3 seconds
    },
  },
};
</script>

<style>
@keyframes slideUpp {
  0% {
    transform: translateY(100%);
  }
  100% {
    transform: translateY(0);
  }
}

.animate-slide-upp {
  animation: slideUpp 2s ease forwards;
}
</style>
