<template>
  <div class="top">
  <img alt="top_picture" src="../assets/top.png" class="top">
  <h1 class="kasaneru">シャキルスタジオ<br>メンバー募集中！</h1>
  </div>
</template>

<script>
export default {
  name: 'NiceTop'
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
/* *{border:solid 1px red;} */
.top {
  display: block;
  position: relative;
  left: -4px
}

img.top {
  width: 100vw;
  height: 654px;
  object-fit: cover;
}

h1.kasaneru{
  font-family: sans-serif;
  font-size: 500%;
  position: absolute;
  top: 49%;
  left: 0%;
  color: white;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  line-height: 110%;
  padding: 0 3%;
}

</style>
