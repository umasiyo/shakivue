<template>
<html lang="ja"><!--日本語のhtml文書だよの宣言-->
  <head><!--ページ情報記述-->
    <meta charset="UTF-8"><!--文字化けしないために必須-->
    <link rel="icon" type="png" href="./assets/logo_white.png">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=BIZ+UDPGothic:wght@400;700&display=swap" rel="stylesheet">
    <title>シャキルスタジオメンバー募集</title><!--ブラウザタブ、ブックマークしたときのタイトル-->
    <meta name="description" content="シャキルスタジオ（仮）の再始動に際し、新たなメンバーを募集する。"><!--ページの簡単な説明-->
  </head>
  <body>
    <div id="loading">
      <div class="shakilstudio1"><!--ロゴ-->
          <img src="./assets/logo_white.png" alt="ShakilStudio_logo" class="logo">
          <img src="./assets/textlogo_white.png" alt="ShakilStudio_textlogo" class="textlogo">
          <h2>is getting ready.</h2>
      </div>
    </div>
    <div class="main">
      <NiceHeader/>
      <NiceTop/>
      <NiceAbout/>
      <NiceWorks/>
      <NiceRecords/>
      <NiceForm/>
      <NiceFooter/>
      <!-- <HelloWorld/> -->
    </div>
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
const sleep = (time) => new Promise((resolve) => setTimeout(resolve, time));
window.onload=async()=>{
  const loading = document.getElementById('loading')
  await sleep(2000);
  loading.classList.add('loaded')
}
</script>

<style>
#app {
  font-family: "BIZ UDPGothic", sans-serif;
  font-weight: 400;
  font-style: normal;
}
html {
  font-size: 100%;
}/*後でemとかrem使えるようにfont-sizeの基準決めとく。*/
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  overflow-x: hidden;
  scroll-behavior: smooth;
}/*変な余白があると嫌なので。スクロールを滑らかに*/
.main {
  width: 100%;
  height: 100vh;
  background: white;
}
#loading {
  transition: all 1s;
  background: #082B70;
  position: fixed;
  z-index: 9999;
  inset: 0;
  display: grid;
  place-items: center;
}
.shakilstudio1 {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: white;
}
.logo {
  width: 56px;
  height: 56px;
  margin: 24px;
}
.textlogo {
  width: 41ch;
  height: 48px;
  margin-right: 30px;
}/*シャキスタロゴ、インスタロゴのサイズ設定*/
.shakilstudio1 h2 {
  position: relative;
  top: 15px;
}
.loaded {
  opacity: 0;
  visibility: hidden;
}
</style>
