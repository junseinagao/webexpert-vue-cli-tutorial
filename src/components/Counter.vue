<!-- ❗️ .vueファイルの中で、<template>タグは、1つの子しか持てません。❗️ -->
<template>
  <div class="counter"></div>
</template>

<script>
export default {}
</script>

<!-- ❗️ <style scoped>を使うと、CSSのスコープをこの.vueファイルに限定できます! ❗️ -->
<style scoped>
.counter {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: lightgreen;
}
</style>
