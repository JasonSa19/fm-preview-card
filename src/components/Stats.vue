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
    <div class="txt-content">
      <h1>{{ hl }}</h1>
      <p>{{ msg }}</p>

      <div class="stat-counts">
        <span>{{ companycount }}</span>
        <span>{{ templatescount }}</span>
        <span>{{ queriescount }}</span>
      </div>
    </div>
    <div class="image-content">
      <img src="./../assets/img/header-image.jpg" />
    </div>
  </section>
</template>

<style scoped></style>
