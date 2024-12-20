<script setup lang="ts">
import { ref } from "vue";

defineProps(['objects'])


</script>

<template>
  <ul>
    <li v-for="object in objects">{{ object }}</li>
  </ul>
</template>

<style scoped>

</style>