<template>
  <div class="w-11/12 h-full mx-auto">
    <Main />
  </div>
</template>

<script>
import Main from "./components/Main.vue";

export default {
  name: "App",
  components: {
    Main
  }
};
</script>

<style>
@import "../public/build/tailwind.css";
html,
body {
  width: 100%;
  height: 100%;
}
body {
  background-color: #f1f1f1;
}
</style>
