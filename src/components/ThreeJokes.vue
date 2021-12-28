<template>
  <div class="d-grid gap-3">
    <Joke />
    <Joke />
    <Joke />
  </div>
</template>

<script>
import Joke from "./Joke";

export default {
  name: "ThreeJokes",
  components: {
    Joke
  }
}
</script>

<style scoped>

</style>