<template>
<section class="top" id="Top">
  <h1>シャキルスタジオ<br>メンバー募集中！</h1>
  <h2>駆け出しのアナタも、熟練のアナタも大歓迎！</h2>
  <a class="button" href="https://umasiyo.github.io/shakivue/" target="_blank" rel="noopener">制作の依頼をしたい方はこちらへ！</a>
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
/* *{border:solid 1px red;} */
section{ 
  display: block;
  text-align: left; 
  font-family: sans-serif; 
  text-transform: uppercase; 
  color: white; 
  width: 100%;
  height: 100vh;
  background-size: cover;
  background-position: center center;
  background-image: url(../assets/top.png);
  background-repeat: no-repeat;
  object-fit: cover;
  padding-top: 70px;
}
.top h1{
  font-size: 60px;/*min20px,max60px*/
  position: absolute;
  top: 60%;
  left: 18%;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  line-height: 110%;
}
.top h2{
  font-size: 30px;/*min20px,max60px*/
  position: absolute;
  top: 78%;
  left: 18%;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  line-height: 110%;
}
.top h3{
  -ms-writing-mode: tb-rl;
  writing-mode: vertical-rl;
  font-size: 50px;/*min20px,max60px*/
  position: absolute;
  top: 22%;
  right: 18%;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
}
.button{ 
  font-size: 20px;
  background: linear-gradient(to right, #E85BFF, #03F0FF);
  color: white;
  line-height: 40px;
  text-align: center;
  border-radius: 20px;
  width: 450px;
  height: 40px;
  position: absolute;
  top: 86%;
  left: 18%;
  text-decoration: none;
}

</style>
