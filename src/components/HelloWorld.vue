<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>
  <div class="container">
    <div class="profile">
      <p>See my profile hier</p>
      <a href="" target="_blank">My Profile</a>
      <a href="" target="_blank">My Linkedin</a>
    </div>
    <div class="countUpDown">
      <button type="button" @click="count++">Count Up</button>
      <button type="button" @click="count--">Count Down</button>
      <p class="count">Count : {{ count }}</p>
    </div>
  </div>
</template>

<style scoped>
a {
  background-color: #f5f5f5;
  color: #42b983;
  text-decoration: none;
}
a:hover {
  background-color: black;
  color: white;
}
.container {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
.countUpDown {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1rem;
}
.count {
  background-color: gray;
  color: yellow;
  width: 10rem;
  height: 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 1rem;
}
.profile {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1rem;
  border: 0.2rem solid black;
  padding: 1.3rem;
  border-radius: 0.4rem;
}

button {
  width: 10rem;
  border-radius: 0.5rem;
  height: 2rem;
  background-color: white;
  color: navy;
  font-size: 1rem;
  font-weight: bold;
}

button:hover {
  background-color: navy;
  color: white;
}
</style>
