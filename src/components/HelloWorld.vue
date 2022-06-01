<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});

const count = ref(0);
</script>

<template>
  <h1>{{ msg }}</h1>

  <p>
    See my profile hier:
    <a href="" target="_blank">My Profile</a>
    +
    <a href="" target="_blank">My Linkedin</a>
  </p>
  <div class="countUpDown">
    <button type="button" @click="count++">Count Up</button>
    <button type="button" @click="count--">Count Down</button>
    <p>Count : {{ count }}</p>
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
.countUpDown {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1rem;
}
</style>
