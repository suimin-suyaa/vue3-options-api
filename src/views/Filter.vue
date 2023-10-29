<template></template>
<script>
const app = Vue.createApp ({
  data() {
    return {
      price: 1000,
    }
  }
})
app.config.globalProperties.$filters = { 
  //【app.config.globalProperties.$filters】定義によってアプリケーションのどこからでも{{ price | number_format }}として使用することができる

  //app.config...vueアプリケーションの設定を行うオブジェクト
  //globalProperties...グローバルに利用可能なプロパティに設定するためのオブジェクト
  //$filters...フィルターを定義するためのプロパティ名

  number_format(val) {
    return val.toLocaleString(); //3桁区切りにし、通貨形式になっている
  }
}

//表示される値は 1,000になる
const vm = app.mount('#app')
</script>
<style></style>