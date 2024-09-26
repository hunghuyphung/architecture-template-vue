<script setup>

import Title from "@/components/Title.vue";
import map from "@/assets/imgs/map.jpg";
</script>

<template>
  <div id="contact" class="p-32-16">
    <Title title="Contact"></Title>
    <p class="my-15">Lets get in touch and talk about your next project.</p>
    <form action="">
      <input type="text" value="Name" class="contact__input">
      <input type="email" value="Email" class="contact__input my-15">
      <input type="text" value="Subject" class="contact__input my-15">
      <input type="text" value="Comment" class="contact__input my-15">
      <div class="flex justify-start">
        <button class="my-15 p-8-16 bc-black text-white border-none">SEND MESSAGE</button>
      </div>
    </form>
  </div>
  <img :src="map" alt="" class="contact__map block w-full">
</template>

<style scoped>
.contact__input {
  display: block;
  padding: 0.5rem;
  width: 100%;
  border: 1px solid #ccc;
}

.contact__map {
  padding: 0 1rem;
}
</style>