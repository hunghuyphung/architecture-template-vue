<script setup>
import Title from "@/components/Title.vue";
import team1 from "@/assets/imgs/team1.jpg";
import team2 from "@/assets/imgs/team2.jpg";
import team3 from "@/assets/imgs/team3.jpg";
import team4 from "@/assets/imgs/team4.jpg";

const teams = [
  {
    id: 0,
    name: 'John Doe',
    pos: 'CEO & Founder',
    img: team2,
  },
  {
    id: 1,
    name: 'Jane Doe',
    pos: 'Architect',
    img: team1,
  },
  {
    id: 2,
    name: 'Mike Ross',
    pos: 'Architect',
    img: team3,
  },
  {
    id: 3,
    name: 'Dan Star',
    pos: 'Architect',
    img: team4,
  },
];
</script>

<template>
  <div id="about">
    <div class="p-32-16">
      <Title title="About"></Title>
      <p class="my-15">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
        labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut
        aliquip ex ea commodo consequat. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia
        deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et
        dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea
        commodo consequat.</p>
    </div>
    <div class="px-8 flex">
      <div v-for="team in teams" key="team.id" class="about__team-item px-8 w-1-4">
        <img :src="team.img" alt="" class="block w-full grayscale-75">
        <div>
          <h3>{{ team.name }}</h3>
          <p class="my-15">
            {{ team.pos }}
          </p>
          <p class="my-15">
            Phasellus eget enim eu lectus faucibus vestibulum. Suspendisse sodales pellentesque elementum.
          </p>
          <button class="p-8-16 w-full bc-light-gray text-black border-none hover-gray">Contact</button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.about__team-item {
  margin-bottom: 1rem;
  padding-bottom: 1rem;
}
</style>