<template>
  <div></div>
</template>
<script>
  const app = Vue.createApp ({
    data () {
      return {
        // アプリケーションが保持するデータをここに定義する
        message: 'Hello Vue.js!'
      }
    },
    methods: {
      // アプリケーションが持つメソッドをここで定義する
    },
    computed: {
      // アプリケーションが持つ算出プロパティをここで定義する
    },
    watch: {
      // アプリケーションが持つウォッチャをここで定義する
    }
  })
const vm = app.mount ('#app');
</script>
<style></style>