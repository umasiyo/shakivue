<template>
<section class="top" id="Top"><!--headerのナビゲーションの移動先としてid設定-->
  <div class="left"><!--左端を揃えたいテキストまとめた-->
    <h1>シャキルスタジオ<br>メンバー募集中！</h1>
    <h2>駆け出しのアナタも、熟練のアナタも大歓迎！</h2>
    <a class="button" href="https://www.instagram.com/shakilstudio.temp/" target="_blank" rel="noopener">制作の依頼をしたい方はこちらへ！</a>
  </div>
  <h3>見たいのは、<br>何かを本気で作る君</h3>
</section>
</template>

<script>
export default {
  name: 'NiceTop'
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
section{ 
  display: block;
  font-family: sans-serif; 
  text-transform: uppercase;/*すべての文字を大文字にする*/
  color: white; 
  width: 100%;
  height: 100vh;/*表示できる画面の縦100%*/
  background-size: cover;/*背景画像を表示したいアスペクト比に調整*/
  background-position: center center;/*背景画像の真ん中が縦横中央に来るように*/
  background-image: url(../assets/top.png);/*imgurl*/
  object-fit: cover;/*アスペクト比を調整したら、縦方向に圧縮されたので、画像自体を切り抜く形にする。*/
  padding-top: 70px;/*headerのposition:fixed;のせいで常に上70pxが隠れてしまうのを調整。これをしないとナビゲーションから飛んだときにずれてしまう*/
}
.left { position: relative; top: 50%; left: 18%; width: 80%; }/*左端を揃えたいテキストをまとめて位置指定する。width100%のまま,右に18%ずらすとその分空白が生まれるので、width82%以下にする。*/
.left h1{ font-size: 60px;/*min20px,max60px*/ filter: drop-shadow(0px 0px 2px #4f4e4e); line-height: 110%; margin: 0;}/*line-heightは行間設定*/
.left h2{ font-size: 30px;/*min20px,max60px*/ filter: drop-shadow(0px 0px 2px #4f4e4e); margin: 0;}
.button{ 
  font-size: 20px;
  background: linear-gradient(to right, #E85BFF, #03F0FF);/*グラデーション*/
  color: white;
  line-height: 40px;
  text-align: center;
  border-radius: 20px;
  text-decoration: none;
  padding:5px 50px;/*テキスト周りの余白を設定してボタンのサイズを決めれる*/
}
h3{
  position: absolute;/*position:relative;で右端基準で位置設定したかったけどできなかった。topでしかできないので汎用性なくて嫌ですがposition:absolute;使います。*/
  top: 20%;
  right: 18%;
  -ms-writing-mode: tb-rl; writing-mode: vertical-rl;/*文章縦書きにするやつ。意味忘れちゃった調べてくれー*/
  font-size: 50px;/*min20px,max60px*/
  filter: drop-shadow(0px 0px 2px #4f4e4e);
}
</style>
