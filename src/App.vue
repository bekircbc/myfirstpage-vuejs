<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import HelloWorld from "./components/HelloWorld.vue";
</script>

<template>
  <div class="header">
    <img alt="bc logo" src="./assets/icon.png" />
    <h1>Vuejs</h1>
  </div>
  <HelloWorld msg="My First Page with Vuejs" />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.header {
  display: flex;
  justify-content: center;
  align-items: center;
}
img {
  width: 10rem;
  height: 10rem;
}
</style>
