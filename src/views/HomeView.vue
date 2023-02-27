<script setup>
import Header from "../components/HomeView/Header.vue";
</script>

<template>
  <main>
    <Header />
    <h1 v-for="n in 100" :key="n">{{ n }}</h1>
  </main>
</template>

<style scoped></style>
