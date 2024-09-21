<template>
<a href="#Top"><!--ナビゲーションで説明する-->
<div id="bar"></div>
<header>
  <div id="bar"></div>
  <div class="shakilstudio"><!--ロゴ-->
    <a href="https://umasiyo.github.io/shakivue/"><!--aでリンク、herfに飛ぶ先のurl-->
      <img src="../assets/logo_white.png" alt="ShakilStudio_logo" class="logo">
      <img src="../assets/textlogo_white.png" alt="ShakilStudio_textlogo" class="textlogo">
    </a>
  </div>
  <nav><!--ナビゲーション-->
    <ul class="nav">
      <a href="#About"><li>ABOUT</li></a><!--ページ内で移動させたいとき、移動先にid="移動先"で設定。-->
      <a href="#Works"><li>WORKS</li></a><!--リンクにはherf="#移動先"でできる。-->
      <a href="#Records"><li>RECORDS</li></a><!--スクロール動作を入れるためにApp.vueのcssにscroll-behavior: smooth;を入れてある-->
      <a href="#Roles"><li>ROLES</li></a>
      <a href="#Contact"><li>CONTACT</li></a>
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
const sleep = (time) => new Promise((resolve) => setTimeout(resolve, time));
window.onload=async()=>{
  const loading = document.getElementById('loading')
  await sleep(3000);
  loading.classList.add('loaded')
}

const getScrollPercent = () => {
  const scrolled = window.scrollY;
  const pageHeight = document.documentElement.scrollHeight;
  const viewHeight = document.documentElement.clientHeight;
  const percentage = scrolled / (pageHeight - viewHeight) * 100;
  document.querySelector('#bar').style.width = `${percentage}%`; // バックティックに修正
};

window.addEventListener('scroll', getScrollPercent);
</script>

<!--ここでのCSSはこのcomponentでしか使用できない-->
<style scoped>
header { 
  position: fixed;/*ヘッダーを常に画面の上に表示*/
  width: 100%;
  height: 4rem;
  z-index: 1000;/*ヘッダーの上に他の要素が重ならないようにz軸を高めに設定*/
  display: flex;
  align-items: center;/*header内の要素を横並びに。縦中央に揃える。*/
  justify-content: space-between;/*header内の要素を横に均等に並べる*/
}
.shakilstudio a {
  display: flex;
  align-items: center;
  text-decoration: none;
}/*ロゴのimgとtextを横並び、縦中央配置。リンクの装飾を消す*/
.nav {
  display: flex;
  align-items: center;
  font-size: 1.2rem;
  text-transform: uppercase;
  font-weight: 200;
}/*min10px,max23px*//*font-family: Montserrat;*/
/*ナビゲーション横並び。縦中央。*/
.nav li {
  list-style: none;
  padding: 0 2rem;
}/*リストスタイルなし。リストの横並び間隔設定*/
.nav a {
  font-weight: 600;
  color: white;
  text-decoration: none;
  transition: 0.2s;
}/*textの色、リンクの装飾を消す*/
.nav a:hover {
  color: rgba(255, 255, 255, 0.567);
}
.logo {
  width: 35px;
  height: 35px;
  margin: 15px;
}/*シャキスタロゴ、インスタロゴのサイズ設定*/
.textlogo {
  width: 260px;
  height: 30px;
}/*シャキスタロゴ、インスタロゴのサイズ設定*/
#bar {
  z-index: 1000;
  position: fixed;
  background-color: #BCD2FF;
  height: 0.3rem;
}
</style>