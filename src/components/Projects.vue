<template>
  <div>
    <div v-for="project in projects" :key="project.id">
      <div class="w-4/5 mx-auto text-center">
        <div class="w-100 xl:w-3/5 mx-auto bg-gray-500 rounded-xl">
          <Project v-if="project.id === 1" :project="project" class="text-gray-200 m-5 text-left" />
          <Project v-else :project="project" class="text-gray-200 m-5 mt-16 text-left" />
        </div>
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