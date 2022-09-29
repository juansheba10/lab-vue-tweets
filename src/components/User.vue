<script setup>
defineProps({
  user: {
    type: Object,
    default: () => ({
      name: "Michael Jordan",
      handle: "@JumpMan23",
    }),
  },
});
</script>

<template>
  <span class="user">
    <span class="name"> {{ user.name }} </span>
    <span class="handle">{{ user.handle }} </span>
  </span>
</template>
