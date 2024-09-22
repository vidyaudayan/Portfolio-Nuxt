<template>
  <section id="contact" class="min-h-screen bg-cyan-50 py-12 ">
    <!-- Title and Subtitle -->
    <div class="text-center mb-12">
      <h1 class="text-5xl font-bold text-gray-900">Contact</h1>
      <p class="text-lg text-gray-600 mt-2">I’d love to hear from you! Contact me using the form below.</p>
    </div>

    <!-- Contact Section (Two columns) -->
    <div class="max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-8">
      
      <!-- Left Section (Contact Information) -->
      <div class="relative p-8  bg-[url('/assets/images/contact.avif')] text-white rounded-lg shadow-md flex flex-col justify-center">
        <div class="absolute inset-0 opacity-50 bg-gradient-to-r from-gray-700 to-gray-900"></div>
        <div class="relative z-10">
          <h3 class="text-2xl font-bold mb-6">Contact Information</h3>

          <div class="flex items-center mb-4">
            <font-awesome-icon :icon="['fas', 'envelope']" class="text-2xl mr-3" />
            <p class="text-lg">vidyaudayan89@gmail.com</p>
          </div>

         

          <div class="flex items-center mb-4">
           
            <p class="text-lg">5/1679,
Elementary School street Dharmapuri 636705</p>

          </div>
        </div>
      </div>

      <!-- Right Section (Contact Form) -->
      <div class="bg-white p-8 rounded-lg shadow-md">
        <h3 class="text-2xl font-bold mb-6 text-gray-900">Send Me a Message</h3>

        <form>
          <div class="mb-4">
            <label class="block text-sm font-medium text-gray-700">Name</label>
            <input type="text" class="mt-1 w-full p-3 border border-gray-300 rounded-md" placeholder="Your Name" />
          </div>

          <div class="mb-4">
            <label class="block text-sm font-medium text-gray-700">Email</label>
            <input type="email" class="mt-1 w-full p-3 border border-gray-300 rounded-md" placeholder="Your Email" />
          </div>

          <div class="mb-4">
            <label class="block text-sm font-medium text-gray-700">Message</label>
            <textarea class="mt-1 w-full p-3 border border-gray-300 rounded-md  resize-none " rows="5" placeholder="Your Message"></textarea>
          </div>

          <button type="submit" class="w-full bg-gray-900 text-white py-3 rounded-md hover:bg-gray-700 transition">
            Send Message
          </button>
        </form>
      </div>

    </div>
  </section>
</template>


import { faLocationArrow } from '@fortawesome/free-solid-svg-icons';

library.add(faLocationArrow);
<script>

export default {
  data() {
    return {
      // Additional data if necessary
    };
  },
};
</script>

<!-- Styles for the Contact Page -->
<style scoped>
/* Custom styles if needed */
</style>
