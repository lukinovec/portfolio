<template>
  <div
    class="fixed Arrow text-6xl transition duration-300 ease-in-out hover:text-gray-700 transform hover:-translate-y-1 hover:scale-110"
  >
    <a href="#landing" v-smooth-scroll class="arrow p-6 h-6">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 24 24"
        class="icon-arrow-thick-up-circle"
        width="36"
        height="36"
        fill="#718096"
      >
        <circle cx="12" cy="12" r="10" class="primary" />
        <path
          class="secondary"
          fill="white"
          d="M14 12v5a1 1 0 0 1-1 1h-2a1 1 0 0 1-1-1v-5H8a1 1 0 0 1-.7-1.7l4-4a1 1 0 0 1 1.4 0l4 4A1 1 0 0 1 16 12h-2z"
        />
      </svg>
    </a>
    <p class="text-xs"></p>
  </div>
</template>

<script>
export default {
  name: "Arrow"
};
</script>

<style scoped>
.Arrow {
  bottom: 40%;
  left: 5px;
}

.arrow {
  width: 24px;
  height: 24px;
  position: relative;
  top: 50%;
}

.icon-arrow-thick-up-circle {
  transition-property: fill;
  transition-duration: 300ms;
}
.Arrow:hover .icon-arrow-thick-up-circle {
  fill: #4a5568;
}
</style>