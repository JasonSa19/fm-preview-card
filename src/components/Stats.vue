<script setup>
import { ref } from "vue";

defineProps({
  hl: String,
  msg: String,
  statCountOne: String,
  statWordingOne: String,
  statCountTwo: String,
  statWordingTwo: String,
  statCountThree: String,
  statWordingThree: String,
});
</script>

<template>
  <section
    class="flex max-w-[80%] mx-auto my-auto justify-between bg-foreground-dark"
  >
    <div class="txt-content">
      <h1>{{ hl }}</h1>
      <p>{{ msg }}</p>

      <div class="stat-counts">
        <div class="flex flex-col items-start">
          <span>{{ statCountOne }}</span
          ><span>{{ statWordingOne }}</span>
        </div>
        <div class="flex flex-col items-start">
          <span>{{ statCountTwo }}</span
          ><span>{{ statWordingTwo }}</span>
        </div>
        <div class="flex flex-col items-start">
          <span>{{ statCountThree }}</span
          ><span>{{ statWordingThree }}</span>
        </div>
      </div>
    </div>
    <div class="image-content">
      <img src="./../assets/img/header-image.jpg" />
    </div>
  </section>
</template>

<style scoped></style>
