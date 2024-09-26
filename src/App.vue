<script setup>
import Header from "@/components/Header.vue";
import Slider from "@/components/Slider.vue";
import Project from "@/components/Project.vue";
import About from "@/components/About.vue";
import Contact from "@/components/Contact.vue";
import Footer from "@/components/Footer.vue";
</script>

<template>
  <Header></Header>
  <Slider></Slider>
  <div id="container" class="mx-auto p-8-16">
    <Project></Project>
    <About></About>
    <Contact></Contact>
  </div>
  <Footer></Footer>
</template>

<style scoped>
#container {
  max-width: 1564px;
}
</style>
