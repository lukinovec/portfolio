<template>
  <div
    class="fixed footer text-black text-6xl transition duration-300 ease-in-out hover:text-gray-700 transform hover:-translate-y-1 hover:scale-110"
  >
    <a href="#landing" class="arrow p-6 h-6">^</a>
  </div>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style scoped>
.footer {
  bottom: 40%;
  left: -10px;
}

.arrow {
  width: 24px;
  height: 24px;
  position: relative;
  top: 50%;
}
</style>