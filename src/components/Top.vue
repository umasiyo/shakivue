<template>
  <html lang="ja">
    <head>
      <meta charset="UTF-8">
    </head>

    <body>
      <div class="top">
        <img src="../assets/top.png" alt="Top_picture" class="top">
        <h1 class="kasaneru">シャキルスタジオ<br>メンバー募集中！</h1>
        <h2>駆け出しのアナタも、熟練のアナタも大歓迎！</h2>
      </div>
    </body>
  </html>
</template>

<script>
export default {
  name: 'NiceTop'
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
/* *{border:solid 1px red;} */

html{
  font-size: 100%;
}

.top {
  display: block;
  position: relative;
  /*left: -4px*/
}

img.top {
  width: 100lvw;
  height: 100lvh;
  object-fit: cover;
}

.kasaneru{
  font-family: sans-serif;
  font-size: clamp(1.25rem, 0.341rem + 4.55vw, 3.75rem);/*min20px,max60px*/
  position: absolute;
  top: 49%;
  left: 20%;
  color: white;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  line-height: 110%;
  padding: 0 3%;
}

</style>
