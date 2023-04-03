<script setup></script>

<template>
  <div class="header">
    <h1>Welcome to drewssite.top</h1>
    <p>This is my website :)</p>
    <RouterLink to="/about">Learn More!</RouterLink>
  </div>
</template>

<style scoped>
.header {
  background-image: linear-gradient(
      to right,
      rgba(255, 0, 0, 0.5),
      rgba(255, 255, 255, 0.5)
    ),
    linear-gradient(blue, purple);
  padding: 10px;
  display: flex;
  flex-direction: column;
}

.header h1,
p {
  font-family: sans-serif;
}

.header a {
  text-decoration: none;
  color: white;
  background-color: black;
  border-radius: 10px;
  padding: 10px;
  font-family: sans-serif;
  width: fit-content;
  transition: color 0.25s;
  font-weight: bold;
}

.header a:hover {
  color: red;
  transition: color 0.25s;
}
</style>
