<template>
  <div class="flex min-h-full text-xl">
    <div class="text-center m-auto landing">
      <h1 class="text-5xl font-bold">Lukáš Vrba</h1>
      <div class="navigation">
        <a href="#contact" v-smooth-scroll class="inline-block">Contact</a>
        <span class="border-l-2 border-r-2 border-gray-700 mx-4"></span>
        <a href="#projects" v-smooth-scroll class="inline-block">Projects</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Landing"
};
</script>

<style scoped>
</style>