<template>
  <div id="app">
    <Tutorial :style="{ marginTop: 3.75 + 'rem' }"></Tutorial>
  </div>
</template>

<script>
import Tutorial from "@/components/Tutorial.vue"

export default {
  name: "App",
  components: {
    Tutorial,
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
