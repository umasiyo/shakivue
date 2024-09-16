<template>
<section class="top" id="Top"><!--headerのナビゲーションの移動先としてid設定-->
  <div class="left"><!--左端を揃えたいテキストまとめた-->
    <h1>Make it better than when you arrived.</h1>
    <h2>「使う前より美しく」の理念のもと、<br>お客様の依頼・アイデアをより良い物にします。</h2>
  </div>
</section>
</template>

<script>
export default {
  name: 'NiceTop'
}
</script>

<style scoped>
section { 
  display: block;
  color: white;
  width: 100%;
  height: 100vh;/*表示できる画面の縦100%*/
  background-size: cover;/*背景画像を表示したいアスペクト比に調整*/
  background-position: center center;/*背景画像の真ん中が縦横中央に来るように*/
  background-image: url(../assets/top.png);/*imgurl*/
  object-fit: cover;/*アスペクト比を調整したら、縦方向に圧縮されたので、画像自体を切り抜く形にする。*/
  padding-top: 150px;/*headerのposition:fixed;のせいで常に上70pxが隠れてしまうのを調整。*/
  position: relative;/*位置調整の基準にする*/
}
.left {
  position: absolute;
  top: 55%;
  left: 18%;
}/*左端を揃えたいテキストをまとめて位置指定する。width100%のまま,右に18%ずらすとその分空白が生まれるので、width82%以下にする。*/
.left h1 {
  font-size: 3rem;/*min20px,max60px*/
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  margin: 0;
}/*line-heightは行間設定*/
</style>