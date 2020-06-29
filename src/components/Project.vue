<template>
  <div class="w-100 grid grid-rows-1 grid-cols-2">
    <div class="w-100 lg:w-4/5 col-span-2 lg:col-span-1">
      <div class="text p-4">
        <h1 class="font-bold">{{ project.name }}</h1>
        <p class="text-2xl">{{ project.description }}</p>
      </div>
      <div class="w-100 p-4 text-lg">
        <button class="w-1/3 bg-gray-600 p-2 rounded-xl">Try it</button>
        <button class="w-1/3"></button>
        <button class="w-1/3 bg-gray-600 p-2 rounded-xl">GitHub</button>
      </div>
    </div>

    <div class="lg:my-auto lg:w-4/5 hidden lg:block">
      <img :src="project.image" class="rounded-xl" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Project",
  props: ["project"]
};
</script>

<style>
</style>