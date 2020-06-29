<template>
  <div class="w-11/12 h-full mx-auto">
    <Main />
  </div>
</template>

<script>
import Main from "./components/Main.vue";

export let store = {
  debug: true,
  state: {
    message: "Hello!",
    searchtype: "movies",
    search: "",
    users_movies: [],
    results: []
  },
  // Change state
  mutateSearch(newValue) {
    this.state.search = newValue;
  },
  setMessageAction(newValue) {
    if (this.debug) console.log("setMessageAction triggered with", newValue);
    this.state.message = newValue;
  },
  clearMessageAction() {
    if (this.debug) console.log("clearMessageAction triggered");
    this.state.message = "";
  }
};

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
  height: 100%;
}
body {
  background-color: #f1f1f1;
}
</style>
