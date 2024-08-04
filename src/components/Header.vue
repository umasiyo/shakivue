<template>
  <html lang="ja"><!-- 日本語のhtml文書だよの宣言 -->
    <head><!-- ページ情報記述 -->
      <meta charset="UTF-8"><!-- 文字化けしないために必須 -->
      <title>シャキルスタジオメンバー募集</title><!-- ブラウザタブ、ブックマークしたときのタイトル -->
      <meta name="description" content="シャキルスタジオ（仮）の再始動に際し、新たなメンバーを募集する。">
    </head>
    <body><!-- 実際の中身ここからブラウザ上で表示される -->
      <header>
        <div class="shakilstudio">
          <a href="https://umasiyo.github.io/shakivue/">
            <img src="../assets/logo_white.png" alt="ShakilStudio_logo" class="logo">
            <h1>SHAKIL STUDIO</h1>
          </a>
        </div>
        <div>
          <nav class="nav">
            <ul>
              <li><a href="https://vuejs.org" target="_blank" rel="noopener">ABOUT</a></li>
              <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">WORKS</a></li>
              <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">RECORDS</a></li>
              <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">FORM</a></li>
            </ul>
          </nav>
        </div>
        <div class="insta_logo">
          <a href="https://www.instagram.com/" target="_blank" rel="noopener">
            <img src="../assets/ig_logo.png" alt="Instagram_logo" class="logo">
          </a>
        </div>
      </header>
    </body>
  </html>
</template>
<script>
export default {
  name: 'NiceHeader',
}
</script>
<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
html{ font-size: 100%; }
header{
  position: fixed;
  top: 0;
  left: 0;
  margin: 0;
  width: 100%;
  height: 70px;
  z-index: 10;
  background-color: #082B71;
  display: flex;
  align-items: center;
}
.shakilstudio { float: left; }
.shakilstudio a{ display: flex; align-items: center; }
.shakilstudio h1{ color: white; line-height: 70px; float: right; }
.nav{ margin: 0 auto; }
.nav ul{ list-style: none; display: flex; align-items: center; text-align: center; position: relative; }
.nav li{ display: inline-block; float: left; padding: 0; position: relative; }
.nav a{
  display: block;
  line-height: 70px;
  font-family: Montserrat;
  font-size: 14px;/*min10px,max23px*/
  font-weight: 600;
  color: white;
  text-align: center;
  padding: 0 14px;
  text-decoration: none;
}
.insta_logo { float: right; }
img.logo { width: 37px; height: 37px; padding: 15px; }
</style>