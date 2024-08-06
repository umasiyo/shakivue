<template>
<a href="#Top"><!--ナビゲーションで説明する-->
<header>
  <div class="shakilstudio"><!--ロゴ-->
    <a href="https://umasiyo.github.io/shakivue/"><!--aでリンク、herfに飛ぶ先のurl-->
      <img src="../assets/logo_white.png" alt="ShakilStudio_logo" class="logo">
      <h1>SHAKIL STUDIO</h1>
    </a>
  </div>
  <nav><!--ナビゲーション-->
    <ul class="nav">
      <li><a href="#About">ABOUT</a></li><!--ページ内で移動させたいとき、移動先にid="移動先"で設定。-->
      <li><a href="#Works">WORKS</a></li><!--リンクにはherf="#移動先"でできる。-->
      <li><a href="#Records">RECORDS</a></li><!--スクロール動作を入れるためにApp.vueのcssにscroll-behavior: smooth;を入れてある-->
      <li><a href="#Form">FORM</a></li>
    </ul>
  </nav>
  <div class="insta_logo"><!--インスタロゴ-->
    <a href="https://www.instagram.com/shakilstudio.temp/" target="_blank" rel="noopener"><!--target="_blank"で別タブでリンクを開く。rel="noopener"はセキュリティ対策らしい。この2つはセット-->
      <img src="../assets/ig_logo.png" alt="Instagram_logo" class="logo">
    </a>
  </div>
</header>
</a>
</template>

<script>
export default {
  name: 'NiceHeader',
}
</script>

<!--ここでのCSSはこのcomponentでしか使用できない-->
<style scoped>
header{ 
  position: fixed;/*ヘッダーを常に画面の上に表示*/
  width: 100%; height: 70px;
  z-index: 10;/*ヘッダーの上に他の要素が重ならないようにz軸を高めに設定*/
  background-color: #082B71;
  display: flex; align-items: center;/*header内の要素を横並びに。縦中央に揃える。*/
  justify-content: space-between;/*header内の要素を横に均等に並べる*/
}
.shakilstudio a{ display: flex; align-items: center; text-decoration: none; color: white; }/*ロゴのimgとtextを横並び、縦中央配置。リンクの装飾を消す*/
.nav{ display: flex; align-items: center; font-size: 20px; text-transform: uppercase; font-weight: 200; list-style: none; }/*min10px,max23px*//*font-family: Montserrat;*/
/*ナビゲーション横並び。縦中央。リストスタイルなし。*/
.nav li{margin-left: 14px; }/*リストの横並び間隔設定*/
.nav a{ color: white; text-decoration: none; }/*textの色、リンクの装飾を消す*/
img.logo { width: 37px; height: 37px; padding: 15px; }/*シャキスタロゴ、インスタロゴのサイズ設定*/
</style>