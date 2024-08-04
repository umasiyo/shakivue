<template>
<html lang="ja"><!-- 日本語のhtml文書だよの宣言 -->
  <head><!-- ページ情報記述 -->
    <meta charset="UTF-8"><!-- 文字化けしないために必須 -->
    <link rel="icon" type="png" href="../assets/logo_white.png">
    <title>シャキルスタジオメンバー募集</title><!-- ブラウザタブ、ブックマークしたときのタイトル -->
    <meta name="description" content="シャキルスタジオ（仮）の再始動に際し、新たなメンバーを募集する。">
  </head>
  <body>
    <NiceHeader/>
    <NiceTop/>
    <NiceAbout/>
    <NiceWorks/>
    <NiceRecords/>
    <NiceForm/>
    <NiceFooter/>
    <!-- <HelloWorld/> -->
  </body>
</html>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import NiceHeader from './components/Header.vue'
import NiceTop from './components/Top.vue'
import NiceAbout from './components/About.vue'
import NiceWorks from './components/Works.vue'
import NiceRecords from './components/Records.vue'
import NiceForm from './components/Form.vue'
import NiceFooter from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    NiceHeader,
    NiceTop,
    NiceAbout,
    NiceWorks,
    NiceRecords,
    NiceForm,
    NiceFooter
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
html{ font-size: 100%; }
body{ margin: 0; padding: 0; }
</style>
