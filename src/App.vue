<template></template>
<h1>Reaction Timer Game</h1>
<button class @click="start"> Play </button>
<script>

export default {
  name: 'App',
  components: {},
  data() {
    return {
      isPlaying: false,
      delay: null
    }
  },
  methods: {
    start() {
      this.delay = 2000 + Math.random() * 3000
      this.isPlaying = true;
      console.log(delay)
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #444;
  margin-top: 60px;
}
</style>
