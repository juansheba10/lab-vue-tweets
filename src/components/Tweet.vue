<template>
  <div className="tweet">
    <ProfileImage :image="imageFather" />

    <div className="body">
      <div className="top">
        <User v-bind:user="userFather" />
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
import User from "./User.vue";
import TimesStamp from "./TimesStamp.vue";
import ProfileImage from "./ProfileImage.vue";

defineProps({
  messageFather: {
    type: String,
  },
  userFather: {
    type: Object,
  },
  timestampFather: {
    type: String,
  },
  imageFather: {
    type: String,
  },
});
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
