<template>
  <div v-if="joke.type === 'single'" class="p-2 bg-light border">
    <p>{{ joke.joke }}</p>
  </div>
  <div v-else class="p-2 bg-light border">
    <p>{{ joke.setup }}</p>
    <p>{{ joke.delivery }}</p>
  </div>
</template>

<script>
export default {
  name: "Joke",
  data() {
    return {
      joke: {}
    }
  },
  methods: {
    async fetchJoke() {
      fetch('https://v2.jokeapi.dev/joke/Any')
          .then(res => res.json())
          .then(data => this.joke = data)
    },
  },
  async created() {
    this.joke = await this.fetchJoke()
  }
}
</script>

<style scoped>

</style>