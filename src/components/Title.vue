<script setup>
import {defineProps} from 'vue';

const props = defineProps({
  title: {
    type: String,
    required: true
  }
});
</script>

<template>
  <h3 class="title py-16">{{ title }}</h3>
</template>

<style scoped>
.title {
  border-bottom: 1px solid #f1f1f1 !important;
}
</style>