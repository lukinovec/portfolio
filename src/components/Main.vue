<template>
  <div class="text-4xl">
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
        portfolio: {
          id: 2,
          name: "Portfolio",
          description: "The portfolio you are seeing right now",
          image: "https://i.imgur.com/lBp6V2N.png",
          technology: ["HTML5", "CSS3", "Tailwind", "Javascript", "Vue.js"]
        },
        expenses: {
          id: 3,
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
