<template>
  <div class="container mx-auto p-4 mt-8 bg-white shadow-md">
    <h2 class="text-2xl font-bold text-white bg-black p-2">{{ title }}</h2>
    <div class="p-4">
      <p class="text-xl font-semibold text-black">{{ subtitle }}</p>
      <p class="text-gray-700">{{ description }}</p>
      <p class="text-black font-bold">{{ dates }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    subtitle: String,
    description: String,
    dates: String
  }
};
</script>