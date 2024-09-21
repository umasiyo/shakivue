<template>
<section class="about" id="About">
  <div class="toumei"><!--背景写真透明にするやつ-->
    <div class="text">
      <h1>About</h1>
      <h2>シャキルスタジオとは</h2>
      <p>ポスター、動画、webサイトの制作やイベント配信環境の整備など<br>”なんでも”やる学生団体です。<br>依頼を募集し、お客様に寄り添った仕事をしていきます。<br>メンバーは経験値に関係なく興味がある分野にチャレンジし、成長を目指します。</p>
    </div>
  </div>
</section>
</template>
  
<script>
export default {
  name: 'NiceAbout'
}
</script>

<style scoped>
section {
  display: block;
  width: 100%;
  height: 600px;
  /*background-size: cover;
  background-position: center center;
  background-image: url(../assets/countdownhirata_seisakukatei.png);
  background-repeat: no-repeat;
  object-fit: cover;*/
  position: relative;
}
.toumei {
  position: absolute;
  width: 100%;
  height: 600px;
  /*background: rgba(255, 255, 255, 0.567);*/
}/*rgbaが透明にするやつ*/
.text {
  position: relative;
  top: 20%;
  margin: 0;
  padding: 0;
  text-align: center;
}/*textをまとめて位置指定。横中央寄せ。*/
.text h1 {
  font-size: 3rem;
  margin-bottom: 0;
  color: #CC8800;
}
.text h2 {
  font-size: 1.8rem;
  margin-top: 0;
}
.text p {
  font-size: 1.5rem;
}
</style>