<template>
  <footer class="bg-gray-900 text-white py-8">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Footer Top -->
      <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        <!-- Logo and About Section -->
        <div class="text-center md:text-left">
          <h2 class="text-2xl font-bold">Vidyamol Udayan</h2>
          <p class="mt-2 text-gray-400">
            Full Stack Developer passionate about building web applications and solving real-world problems.
          </p>
        </div>

        <!-- Navigation Links -->
        <div class="text-center">
          <h3 class="text-lg font-semibold">Quick Links</h3>
          <nav class="mt-4">
            <ul class="space-y-2">
              <li><a href="#about" class="hover:text-blue-500">About Me</a></li>
              <li><a href="#skills" class="hover:text-blue-500">Skills</a></li>
              <li><a href="#projects" class="hover:text-blue-500">Projects</a></li>
              <li><a href="#contact" class="hover:text-blue-500">Contact</a></li>
            </ul>
          </nav>
        </div>

        <!-- Social Media and Contact Info -->
        <div class="text-center md:text-right">
          <h3 class="text-lg font-semibold">Contact</h3>
          <div class="flex justify-center md:justify-end space-x-4 mt-4">
            <!-- Social Media Icons -->
            <a href="https://github.com/your-profile" target="_blank" class="text-gray-400 hover:text-white">
              <font-awesome-icon :icon="['fab', 'github']" class="text-2xl"/>
            </a>
            <a href="https://linkedin.com/in/your-profile" target="_blank" class="text-gray-400 hover:text-white">
              <font-awesome-icon :icon="['fab', 'linkedin']" class="text-2xl"/>
            </a>
            <a href="mailto:your-email@example.com" class="text-gray-400 hover:text-white">
              <font-awesome-icon :icon="['fas', 'envelope']" class="text-2xl"/>
            </a>
          </div>
          <!-- Contact Information -->
          <div class="mt-4 text-gray-400">
          
            <p> vidyaudayan89@gmail.com</p>
            <p class="mt-2"> Dharmapuri,Tamil Nadu, India</p>
          </div>
        </div>
      </div>

      <!-- Footer Bottom (Copyright) -->
      <div class="mt-8 border-t border-gray-700 pt-4 text-center">
        <p class="text-gray-500 text-sm">&copy; 2024 Vidyamol Udayan. All rights reserved.</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  components: {
   
    FontAwesomeIcon: () => import('@fortawesome/vue-fontawesome')
  }
}
</script>

