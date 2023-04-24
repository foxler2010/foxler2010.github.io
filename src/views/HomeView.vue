<script setup>
import HeaderComponent from "../components/HeaderComponent.vue";
</script>

<template>
  <main>
    <HeaderComponent
      title="Welcome to drewssite.top"
      subtext="This is my website :)"
      buttonText="Learn More!"
    />
    <h1 v-for="n in 100" :key="n">{{ n }}</h1>
  </main>
</template>

<style scoped></style>
