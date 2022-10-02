<script setup>
import Timestamp from "./Timestamp.vue";
defineProps({
  user: {
    type: Object,
    default: () => ({
      name: "Nasa",
      handle: "@Nasa",
    }),
  },
  timestamp: {
    type: String,
  },
});
</script>

<template>
  <div class="top">
    <span class="name">{{ user.name }}</span>
    <span class="handle">{{ user.handle }}</span>
    <Timestamp v-bind:timestamp="timestamp" />
  </div>
</template>
