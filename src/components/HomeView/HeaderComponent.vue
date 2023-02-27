<script setup>
import { RouterLink } from "vue-router";
</script>

<template>
  <div class="header">
    <div class="box">
      <h1>Welcome to drewssite.top</h1>
      <p>This is my website :)</p>
      <div id="box-button-container">
        <RouterLink to="/about" class="box-button real-box-button">Learn more!</RouterLink>
        <RouterLink to="/about" class="box-button box-button-cover">Learn more!</RouterLink>
      </div>
    </div>
  </div>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: center;
  background-image: linear-gradient(
      to right,
      rgba(255, 0, 0, 0.5),
      rgba(255, 255, 255, 0.5)
    ),
    linear-gradient(blue, purple);
}

.box {
  display: flex;
  flex-flow: column;
  gap: 0.5em;
  background-color: black;
  padding: 2em;
  border-radius: 1em;
  margin-top: 10%;
  margin-bottom: 10%;
}

.box h1,
p {
  font-family: sans-serif;
  color: white;
  margin-top: 0;
}

#box-button-container {
  position: relative;
}

.box-button {
  background-color: white;
  padding: 1em;
  border: none;
  border-radius: 1em;
  color: black;
  font-size: 1em;
  font-family: sans-serif;
  text-decoration: none;
  font-weight: bold;
}

.real-box-button {
  background-image: linear-gradient(to right, red, yellow);
}

.box-button-cover {
  position: absolute;
  transform: translate(-100%, -30%);
  opacity: 1;
  transition: opacity 0.5s;
  background-image: linear-gradient(to right, yellow, red);
}

.box-button-cover:hover {
  transition: opacity 0.5s;
  opacity: 0;
}
</style>
