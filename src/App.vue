<template>
  <div id="app">
    <Tutorial :style="{ marginTop: 3.75 + 'rem' }"></Tutorial>
    <Counter></Counter>
  </div>
</template>

<script>
import Tutorial from "@/components/Tutorial.vue"
import Counter from "@/components/Counter.vue"
export default {
  name: "App",
  components: {
    Tutorial,
    Counter,
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
