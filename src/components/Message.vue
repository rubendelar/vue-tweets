<template>
  <p class="message">
    {{ message }}
  </p>
</template>

<script setup>
defineProps({
  message: {
    type: String,
    default: "Lets climb to the moon, oh ohh, let's fly to the tide...",
  },
});
</script>
