<template>
  <div class="results">
    <p>Reaction time: {{ time }} ms</p>
  </div>
</template>

<script>
export default {
  props: {
    time: { type: Number }
  }
}
</script>
