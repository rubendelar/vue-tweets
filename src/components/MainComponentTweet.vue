<template>
  <div class="tweet">
    <UsersImage
      :image="userImageFather"
      :imageAlt="`${userNameFather.name} - profile image`"
    />

    <div class="body">
      <div class="top">
        <UsersName :user="userNameFather" :timestamp="timestampFather" />
      </div>
      <Message v-bind:message="messageFather" />
      <Actions />
    </div>

    <i class="fas fa-ellipsis-h"></i>
  </div>
</template>

<script setup>
import Actions from "./Actions.vue";
import Message from "./Message.vue";
import Timestamp from "./Timestamp.vue";
import UsersImage from "./UsersImage.vue";
import UsersName from "./UsersName.vue";

defineProps({
  messageFather: {
    type: String,
  },
  timestampFather: {
    type: String,
  },
  userNameFather: {
    type: Object,
  },
  userImageFather: {
    type: String,
  },
  imageAltFather: {
    type: String,
  },
});
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
