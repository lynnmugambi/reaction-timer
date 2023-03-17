<template>
  <div class="results">
    <p>Reaction time: {{ score }} ms</p>
    <p class="rank">{{ rank }}</p>
  </div>
</template>

<script>
export default {
  props: {
    score: { type: Number }
  },
  data() {
    return {
      rank: null
    }
  },
  mounted() {
    this.score < 250 ? this.rank = 'Ninja Fingers' : this.score < 550 ? this.rank = 'Rapid Reactions' : this.rank = 'Too slow bro!'
  },
}
</script>

<style>
.rank {
  font-size: 1.4em;
  color: #0faf87;
  font-weight: bold;
}
</style>
