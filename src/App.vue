<template>
  <div class="container">
    <h1>Three Jokes</h1>
    <ThreeJokes />
  </div>
</template>

<script>
import ThreeJokes from "@/components/ThreeJokes";

export default {
  name: 'App',
  components: {
    ThreeJokes
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
