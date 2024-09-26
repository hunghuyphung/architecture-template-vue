<script setup>
import Title from "@/components/Title.vue";
import house2 from "@/assets/imgs/house2.jpg";
import house3 from "@/assets/imgs/house3.jpg";
import house4 from "@/assets/imgs/house4.jpg";
import house5 from "@/assets/imgs/house5.jpg";

const projectTops = [
  [
    {
      img: house2,
      projectName: 'Summer House'
    },
    {
      img: house3,
      projectName: 'Brick House'
    },
    {
      img: house4,
      projectName: 'Renovated'
    },
    {
      img: house5,
      projectName: 'Barn House'
    },
  ],
  [
    {
      img: house3,
      projectName: 'Brick House'
    },
    {
      img: house4,
      projectName: 'Renovated'
    },
    {
      img: house5,
      projectName: 'Barn House'
    },
    {
      img: house2,
      projectName: 'Summer House'
    },
  ],
]
</script>

<template>
  <div id="project">
    <div class="p-32-16">
      <Title title="Projects"></Title>
    </div>
    <div v-for="projectTop in projectTops" class="px-8">
      <div class="flex">
        <div v-for="project in projectTop" class="project__item px-8 w-1-4">
          <div class="relative">
            <img :src="project.img" alt="" class="block w-full">
            <div class="display-top-left p-8-16 bc-black text-white">{{ project.projectName }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.project__item {
  margin-bottom: 1rem;
}
</style>