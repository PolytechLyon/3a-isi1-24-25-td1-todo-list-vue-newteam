<script setup lang="ts">
import List from "./components/List.vue";
import { ref } from "vue";

const objs = ref([]);
const text = ref('');

function addObject() {
  objs.value.push(text.value);
}
</script>

<template>
  <div>
    <List :objects="objs"/>
    <input id="input" type="text" v-model="text">
    <button @click="addObject()">Add</button>
    <button>Modify</button>
  </div>
</template>

<style scoped>

</style>
