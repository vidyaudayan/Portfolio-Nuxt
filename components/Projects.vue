<template>
  <section id="projects" class="px-4 py-12 bg-gray-100">
    <h2 class="text-center text-4xl font-bold mb-10">Projects</h2>
    
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
      <div v-for="(project, index) in projects" :key="index" class="bg-white shadow-lg rounded-lg overflow-hidden hover:shadow-2xl transition-shadow duration-300">
        <!-- Project Image -->

     

        <div class="bg-white p-4 rounded-lg ">
  <div class="p-4 border border-gray-300 rounded-lg">
    <img :src="project.image" alt="Project Image" class="w-full h-48 object-cover rounded-md">
  </div>
</div>

       
        
        <!-- Project Content -->
        <div class="p-4">
          <!-- Project Title -->
          <h3 class="text-xl font-semibold mb-2">{{ project.title }}</h3>

          <!-- Project Description -->
          <p class="text-gray-700">
            {{ project.shortDescription }}
          </p>

          <!-- Read More/Read Less toggle -->
          <div v-if="project.showMore" class="mt-2 text-gray-600">
            {{ project.longDescription }}
          </div>

          <button
            @click="toggleReadMore(index)"
            class="mt-4 bg-black text-white p-1 px-2 rounded-md text-sm hover:bg-gray-600 "
          >
            {{ project.showMore ? "Read Less" : "Read More" }}
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          title: 'E-commerce Website',
          image: '/assets/images/project1.png', // Replace with actual project image
          shortDescription: 'An online platform for shopping with secure payments.',
          longDescription: 'This e-commerce platform integrates Stripe for secure payments, features a robust admin panel for managing orders and products, and has a dynamic search and filtering system.',
          showMore: false
        },
        {
          title: 'Tourism Landing page ',
          image: '/assets/images/project7.png',
          shortDescription: 'Landing page for a travel and tourism website using React and features a dynamic carousel designed with React Slick',
          longDescription: ' also integrated EmailJS into the contact form to streamline communication and ensure a smooth user experience.',
          showMore: false
        },
        {
          title: 'Portfolio Website',
          image: 'assets/images/project3.png',
          shortDescription: 'My personal portfolio showcasing my skills and projects.',
          longDescription: 'This portfolio website was built using React and TailwindCSS. It features a fully responsive design, interactive components, and optimized performance.',
          showMore: false
        },
         {
          title: 'Functional contact form using EmailJS',
          image: 'assets/images/project4.png',
          shortDescription: 'EmailJS offers a seamless solution for sending emails ',
          longDescription: 'directly from client-side JavaScript without the need for server side code',
          showMore: false
        },
         {
          title: 'Healthy Weight Calculator',
          image: 'assets/images/project5.png',
          shortDescription: 'This tool empowers individuals on their wellness journey',
          longDescription: 'by providing accurate and personalized insights into achieving a healthy weight and BMI value ',
          showMore: false
        },
        {
          title: 'Pagination',
          image: 'assets/images/project6.png',
          shortDescription: 'It helps to navigate through large datasets, enhancing user experience',
          longDescription: 'With an extensive catalog of mock products the fake store API supports fetching products for the pages ',
          showMore: false
        },
        // Add more projects as needed
      ]
    };
  },
  methods: {
    toggleReadMore(index) {
      this.projects[index].showMore = !this.projects[index].showMore;
    }
  }
};
</script>

<style scoped>
/* Custom hover effect for cards */
.card-hover:hover {
  transform: scale(1.05);
  transition: transform 0.3s ease-in-out;
}
</style>
