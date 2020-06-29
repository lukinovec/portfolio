<template>
  <div>
    <h1 class="font-bold">Projects</h1>
    <div class="w-100" v-for="project in projects" :key="project.id">
      <div class="w-4/5 xl:w-2/5 bg-gray-500 rounded-xl">
        <Project :project="project" class="text-gray-200 m-5 mt-16" />
      </div>
      <div class="w-4/5">
        <div class="text-gray-200 inline-block" v-for="tech in project.technology" :key="tech">
          <div class="text-lg m-2 p-1 rounded-lg border border-black text-black">{{ tech }}</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Project from "./Project.vue";
export default {
  name: "Projects",
  components: { Project },
  props: ["projects"]
};
</script>

<style>
</style>