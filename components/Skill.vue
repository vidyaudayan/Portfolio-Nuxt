<template>
  <section id="skills" class="px-8 py-12">
    <h2 class="text-3xl font-bold text-center mb-6">Skills</h2>
    
    <!-- Technical Skills Section -->
    <div class="mb-10">
     
      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Skill Bars -->
        <div v-for="skill in technicalSkills" :key="skill.name" class="p-4 bg-slate-300 hover:bg-slate-400 shadow-md rounded-lg">
          <div class="flex items-center justify-between mb-2">
            <span class="text-xl font-semibold">{{ skill.name }}</span>
            
            <font-awesome-icon :icon="skill.icon" class="text-2xl"></font-awesome-icon>
          </div>
          <div class="relative w-full h-2 bg-gray-300 rounded">
            <div :style="{ width: skill.proficiency + '%' }" class="absolute h-2 bg-cyan-500 rounded"></div>
            <span class="absolute text-xs right-0 -top-5 text-gray-700">{{ skill.proficiency }}%</span>
          </div>
        </div>
      </div>
    </div>

    <!-- Soft Skills Section -->
  
  </section>
</template>

<script setup>


const technicalSkills = [
  { name: 'HTML', proficiency: 95, icon: ['fab', 'html5'] },
  { name: 'CSS', proficiency: 90, icon: ['fab', 'css3-alt'] },
  { name: 'JavaScript', proficiency: 85, icon: ['fab', 'js'] },
  { name: 'React', proficiency: 80, icon: ['fab', 'react'] },
  { name: 'Node.js', proficiency: 75, icon: ['fab', 'node-js'] },
  { name: 'MongoDB', proficiency: 70, icon: ['fas', 'database'] },
];

</script>

<style scoped>
/* Custom styles can go here */
</style>
