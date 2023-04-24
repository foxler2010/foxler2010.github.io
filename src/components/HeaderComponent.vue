<script setup>
defineProps({
  title: {
    type: String,
    required: true,
  },
  subtext: {
    type: String,
    required: false,
    default: "",
  },
  buttonText: {
    type: String,
    required: true,
  },
});
</script>

<template>
  <div class="header">
    <h1>{{ title }}</h1>
    <p v-if="subtext.length > 0">{{ subtext }}</p>
    <RouterLink to="/about">{{ buttonText }}</RouterLink>
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
