<template>
  <html lang="ja"><!-- 日本語のhtml文書だよの宣言 -->
    <head><!-- ページ情報記述 -->
      <meta charset="UTF-8"><!-- 文字化けしないために必須 -->
      <title>シャキルスタジオメンバー募集</title><!-- ブラウザタブ、ブックマークしたときのタイトル -->
      <meta name="description" content="シャキルスタジオ（仮）の再始動に際し、新たなメンバーを募集する。">
    </head>

    <body><!-- 実際の中身ここからブラウザ上で表示される -->
      <header>
        <div class="logo">
          <a href="https://umasiyo.github.io/shakivue/">
            <img src="../assets/logo_white.png" alt="ShakilStudio_logo">
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
        <div>
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
  background-color: #082B71;
  display: flex;
  flex-wrap: nowrap;
  align-items: center;
  justify-content: space-between;
}
.logo h1{ line-height:70px; color: white; float: right; }
.nav ul{ list-style: none; }
.nav li{ float: left; padding: 0; }
.nav li a{
  display: block;
  line-height: 70px;
  font-family: Montserrat;
  font-size: 14px;/*min10px,max23px*/
  font-weight: 600;
  color: white;
  padding: 0 14px;
  text-decoration: none;
}
img.logo { width: 37px; height: 37px; padding: 15px; }
</style>
