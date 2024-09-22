<template>
  <div>
    <Header />
    <main class="pt-16"> <!-- Adjust padding to avoid overlap with the fixed header -->
      <nuxt />

    </main>
  </div>
</template>

<script>
import Header from '~/components/Header.vue'; // Import the Header component

export default {
  components: {
    Header,
  },
};
</script>

<style>
/* Additional global styles if needed */
</style>
