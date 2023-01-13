<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
    <RouterLink to="/work">Work</RouterLink>
    <RouterLink to="/contact">Contact</RouterLink>
  </nav>
</template>

<style scoped>
nav {
  padding-top: 10px;
  padding-bottom: 10px;
  background-color: darkblue;
}

a {
  padding-top: 10px;
  padding-bottom: 10px;
  padding-left: 5px;
  padding-right: 5px;
  color: white;
  text-decoration: none;
  font-weight: bold;
  font-family: sans-serif;
  transition: background-color 0.25s;
}

a:hover {
  background-color: darkcyan;
  transition: background-color 0.25s;
}

a:current {
  background-color: darkmagenta;
}
</style>
