<script setup>
import { ref } from "vue";
import { RouterView } from "vue-router";
import Nav from "./components/Nav.vue";

const randomState = ref("");
</script>

<template>
  {{ randomState }}
  <button @click="randomState = 'hello there'">Click me</button>
  <div>
    <Nav />
    <RouterView />
  </div>
</template>
