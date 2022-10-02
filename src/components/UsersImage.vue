<template>
  <img v-bind:src="image" class="profile" :alt="imageAlt" />
</template>

<script setup>
defineProps({
  image: {
    type: String,
    default:
      "https://upload.wikimedia.org/wikipedia/commons/thumb/e/e5/NASA_logo.svg/1200px-NASA_logo.svg.png",
  },
  imageAlt: {
    type: String,
    default: "To The Moon!",
  },
});
</script>
