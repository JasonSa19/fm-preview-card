<script setup>
import { ref } from "vue";

defineProps({
  hl: String,
  msg: String,
  companycount: String,
  templatescount: String,
  queriescount: String,
});
</script>

<template>
  <section>
    {{ msg }}
  </section>
</template>

<style scoped></style>
