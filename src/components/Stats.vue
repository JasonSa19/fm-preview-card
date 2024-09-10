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
    class="flex max-w-[80%] mx-auto my-auto justify-between bg-foreground-dark rounded-xl"
  >
    <div class="p-24 txt-content basis-7/12">
      <h1 class="mb-6">{{ hl }}</h1>
      <p class="mb-24">{{ msg }}</p>

      <div class="flex justify-between stat-counts">
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
    <div class="image-content basis-5/12">
      <img
        class="object-cover w-full h-full rounded-r-xl"
        src="./../assets/img/header-image.jpg"
      />
    </div>
  </section>
</template>

<style scoped></style>
