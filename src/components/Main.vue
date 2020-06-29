<template>
  <div class="text-4xl">
    <!-- <div class="w-5/12 p-48 absolute mt-5 bg-gray-500 rounded-xl">
      <h1 class="text-6xl text-gray-200">Lukáš Vrba</h1>
    </div>
    <div class="absolute right-0 mt-6">
      <h1 class="text-5xl text-gray-200">Projects</h1>
      <Project class="text-gray-300 w-1/4 p-24 bg-gray-600 rounded-xl" />
    </div>-->
    <Projects :projects="projects" />
  </div>
</template>

<script>
import Projects from "./Projects.vue";
export default {
  name: "Main",
  components: { Projects },
  data: function() {
    return {
      projects: {
        djangoshop: {
          id: 1,
          name: "DjangoShop",
          description: "Web app where users buy or sell fictive items",
          image: "https://i.imgur.com/4m4qUgb.png",
          technology: ["HTML5", "CSS3", "Bootstrap 4", "Python", "Django"]
        },
        expenses: {
          id: 2,
          name: "Expenses",
          description: "Web app for tracking your expenses and earnings",
          image: "https://i.imgur.com/4m4qUgb.png",
          technology: [
            "HTML5",
            "CSS3",
            "Tailwind",
            "Javascript",
            "Vue.js",
            "PHP 7"
          ]
        }
      }
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
