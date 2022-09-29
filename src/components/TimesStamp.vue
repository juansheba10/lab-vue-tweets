<template>
  <span className="timestamp">{{ timesStamp }}</span>
</template>

<script setup>
defineProps({
  timesStamp: {
    type: String,
    default: () => {
      let date = new Date();
      return date.toISOString().split("T")[0];
    },
  },
});
</script>

>
