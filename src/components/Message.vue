<template>
  <p className="message">{{ message }}</p>
</template>

<script setup>
defineProps({
  message: {
    type: String,
    default: "Generic tweet",
  },
});
</script>
