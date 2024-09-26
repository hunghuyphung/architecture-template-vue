<script setup>

</script>

<template>
  <div id="a-header" class="p-8-16 flex justify-between bc-white">
    <a href="#" class="p-8-16 none-underline tracking-wide text-black hover-gray">
      <b>BR</b>
      Architects
    </a>
    <div>
      <a href="#" class="p-8-16 inline-block none-underline tracking-wide text-black hover-gray">
        Projects
      </a>
      <a href="#" class="p-8-16 inline-block none-underline tracking-wide text-black hover-gray">
        About
      </a>
      <a href="#" class="p-8-16 inline-block none-underline tracking-wide text-black hover-gray">
        Contact
      </a>
    </div>
  </div>
</template>

<style scoped>
#a-header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1;
  box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.16), 0 2px 10px 0 rgba(0, 0, 0, 0.12);
}
</style>