<script setup>
import HeaderComponent from "../components/HomeView/HeaderComponent.vue";
</script>

<template>
  <main>
    <HeaderComponent />
    <h1 v-for="n in 100" :key="n">{{ n }}</h1>
  </main>
</template>

<style scoped></style>
