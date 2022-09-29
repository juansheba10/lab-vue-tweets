<template>
  <img
    referrerpolicy="no-referrer"
    v-bind:src="image"
    className="profile"
    alt="profile"
  />
</template>

<script setup>
defineProps({
  image: {
    type: String,
    default:
      "https://upload.wikimedia.org/wikipedia/commons/a/ae/Michael_Jordan_in_2014.jpg",
  },
});
</script>
