<template>
  <div class="bg-white shadow-md p-4 mt-4 flex justify-center font-bold">
    <div class="w-full max-w">
      <h2 class="text-2xl  text-white bg-black p-2 text-center">Навички</h2>
      <ul class="items-center mt-2">
        <li v-for="(skill, index) in skills" :key="index" class="flex items-center mb-5 justify-center">
          <div class="w-24 flex items-center justify-center">{{ skill.name }}</div>
          <div class="flex ml-4">
            <div v-for="i in 5" :key="i" class="w-6 h-6 border border-gray-300 mr-1 relative">
              <div v-if="i <= skill.level" class="bg-black absolute inset-0"></div>
            </div>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        { name: 'Java Spring Boot', level: 4 },
        { name: 'Vue.js', level: 3 },
        { name: 'HTML, CSS', level: 4 },
        { name: 'MySql', level: 2 },
        { name: 'Git', level: 5 }
      ]
    };
  }
};
</script>