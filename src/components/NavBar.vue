<script setup></script>

<template>
  <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
  </nav>
</template>

<style scoped>
nav {
  padding-top: 10px;
  padding-bottom: 10px;
  background-color: darkblue;
}

RouterLink {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

RouterLink:hover {
  background-color: darkviolet;
  transition: background-color 2s;
}
</style>
