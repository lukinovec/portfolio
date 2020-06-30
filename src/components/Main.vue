<template>
  <div class="relative">
    <Landing class="h-screen" id="landing" />
    <Projects class="text-4xl" id="projects" :projects="projects" />
    <Contact class="h-screen" id="contact" />
    <Footer class="w-100" />
  </div>
</template>

<script>
import Projects from "./Projects.vue";
import Contact from "./Contact.vue";
import Landing from "./Landing.vue";
import Footer from "./Footer.vue";

export default {
  name: "Main",
  components: { Projects, Contact, Landing, Footer },
  data: function() {
    return {
      projects: {
        djangoshop: {
          id: 1,
          name: "DjangoShop",
          description: "Web app where users buy or sell fictive items",
          image: "https://i.imgur.com/4m4qUgb.png",
          technology: ["HTML5", "CSS3", "Bootstrap 4", "Python", "Django"],
          live: "https://cooldjangoshop.herokuapp.com/"
        },
        portfolio: {
          id: 2,
          name: "Portfolio",
          description: "The portfolio you are seeing right now",
          image: "https://i.imgur.com/lBp6V2N.png",
          technology: ["HTML5", "CSS3", "Tailwind", "Javascript", "Vue.js"],
          live: "#"
        },
        expenses: {
          id: 3,
          name: "Expenses",
          description: "Web app for tracking your expenses and earnings",
          image: "https://i.imgur.com/vIO88vm.png",
          technology: [
            "HTML5",
            "CSS3",
            "Tailwind",
            "Javascript",
            "Vue.js",
            "PHP 7"
          ],
          live: "#"
        },
        keeptrack: {
          id: 4,
          name: "KeepTrack",
          description: "Search your TV shows or books and track your progress",
          image: "https://i.imgur.com/ehJL05k.png",
          technology: [
            "HTML5",
            "CSS3",
            "Bootstrap 4",
            "Javascript",
            "jQuery",
            "PHP",
            "Laravel 7"
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
