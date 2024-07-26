<template>
    <div class="bg-white p-4 rounded-lg shadow-md mt-2">
      <h3 class="text-white bg-black text-2xl p-2 text-lg font-bold">Мови</h3>
      <ul class="mt-2">
        <li v-for="language in languages" :key="language.name" class="flex justify-between text-black text-lg mx-80  mt-5">
          <span>{{ language.name }}</span>
          <span>{{ language.level }}</span>
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        languages: [
          { name: 'English', level: 'Середній' },
          { name: 'Українська', level: 'Рідна' },
          { name: 'Російська', level: 'Середній' }
        ]
      };
    }
  };
  </script>