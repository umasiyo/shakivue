<template>
<section class="about" id="About">
  <div class="toumei">
    <div class="text">
      <h1>About</h1>
      <h2>シャキルスタジオって何でしたっけ</h2>
      <p>シャキルスタジオ（仮）とは、<br>ポスター、動画、webサイト等の制作を行う団体です。<br>依頼者に寄り添い、想像を超える作品を目指します。</p>
    </div>
  </div>
</section>
</template>
  
<script>
export default {
  name: 'NiceAbout'
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
/* *{border:solid 1px red;} */
section{
  display: block;
  width: 100%;
  height: 600px;
  background-size: cover;
  background-position: center center;
  background-image: url(../assets/countdownhirata_seisakukatei.png);
  background-repeat: no-repeat;
  object-fit: cover;
}
.toumei{ width: 100%; height: 600px; background-color: rgba(255, 255, 255, 0.567);}
.text{ position: relative; top: 25%; margin: 0; padding: 0;}
.text h1{font-size: 60px; color: black; margin-bottom: 0}
.text h2{font-size: 30px; color: #314F87; margin-top: 0;}
.text p{font-size: 25px; color: black;}
</style>