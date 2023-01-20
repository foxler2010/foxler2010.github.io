<script setup></script>

<template>
  <main>
    <div class="header">
      <img src="../assets/splash.jpg" />
      <div class="box">
        <h1>Welcome to drewssite.top</h1>
      </div>
    </div>
    <h1 v-for="n in 100" :key="n">{{ n }}</h1>
  </main>
</template>

<style scoped>
.header {
  background-color: red;
}

.header img {
  position: absolute;
  width: 100%;
}

.box {
  background-image: linear-gradient(to bottom right,purple, blue, purple);
  padding: 2em;
  border-radius: 1em;
  position: absolute;
  top: 25%;
  bottom: 25%;
  left: 10%;
  right: 10%;
}
.box:hover {

}
.box h1 {
  text-align: center;
  font-family: sans-serif;
}

</style>
