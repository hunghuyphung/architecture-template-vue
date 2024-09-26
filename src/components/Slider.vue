<script setup>
import architect from "@/assets/imgs/architect.jpg";
</script>

<template>
  <div id="slider" class="mx-auto relative">
    <img :src="architect" alt="" class="block">
    <div class="display-middle">
      <h1>
      <span class="p-8-16 bc-black text-white opacity-75">
        <b class="tracking-wide">BR</b>
      </span>
        <span class="text-white tracking-wide"> Architects</span>
      </h1>
    </div>
  </div>
</template>

<style scoped>
#slider {
  max-width: 93.75rem;
}
</style>