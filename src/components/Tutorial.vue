<template>
  <!-- ❗️ .vueファイルの中で、<template>タグは、1つの子しか持てません。❗️ -->
  <div class="tutorial">
    <div>
      <h1 @mouseover="fire">
        {{ icon }}
        {{ courseName }}コース Vue CLI チュートリアル
        {{ icon }}
      </h1>
      <p>
        Vue CLIでの開発は、new
        Vueを使った開発と異なる部分が数点ありますが、より便利に開発できます。<br />
        このTutorialコンポーネントを参考にして、いくつかのアプリを.vueファイルで開発してみましょう!
      </p>
    </div>
  </div>
</template>

<script>
// ❗️ export dafaultを用いてnew Vue({...})に書いてた内容をexportします。決まった書き方として覚えてよいでしょう。❗️
export default {
  // ❗️ .vueファイルでは、dataは、data () { return {} }の様に書きます。❗️
  data() {
    return {
      courseName: "WebExpert",
      icon: "🧨",
    }
  },
  // 他の methodsやcomputed等は、new Vueと一緒です。
  methods: {
    fire() {
      if (this.icon === "🔥") {
        this.icon = "🧨"
      } else if (this.icon === "🧨") {
        this.icon = "🔥"
      }
    },
  },
}
</script>

<!-- ❗️ <style scoped>を使うと、CSSのスコープをこの.vueファイルに限定できます! ❗️ -->
<style scoped>
.tutorial {
  text-align: center;
}
</style>
