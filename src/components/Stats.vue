<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1
    class="text-5xl font-black text-transparent bg-gradient-to-r from-green-600 to-sky-400 bg-clip-text selection:bg-transparent"
  >
    {{ msg }}
  </h1>
</template>

<style scoped></style>
