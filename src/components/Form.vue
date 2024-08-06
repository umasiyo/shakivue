<template>
<section class="form" id="Form">
  <div class="text">
    <h1>Form</h1>
    <h2>参加したい？歓迎するよ！</h2>
  </div>
  <ul class="zukei">
    <li></li>
    <li></li>
    <li></li>
    <li></li>
  </ul>
  <p class="zukei setumei"></p>
  <a class="button" href="https://umasiyo.github.io/shakivue/" target="_blank" rel="noopener">制作の依頼をしたい方はこちらへ！</a>
</section>
</template>
  
<script>
export default {
  name: 'NiceForm'
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
/* *{border:solid 1px red;} */
section{ width: 100%; height: 700px; background-color: white; }
.text{ width: 80%; text-align: left; position: relative; top: 15%; left: 18%; margin: 0; padding: 0;}
.text h1{ font-size: 60px; color: black; margin-bottom: 0; }
.text h2{ font-size: 30px; color: #314F87; margin-top: 0; }
.form ul{list-style: none; position: relative; top: 15%; left: 18%;}
.form li{background-color: #d9d9d9; width: 70px; height: 70px; border-radius: 50%; margin-bottom: 10px;}
.zukei{ float: left;}
.setumei{ width: 600px; height: 320px; background-color: #d9d9d9; 
list-style: none; position: relative; top: 15%; left: 18%; margin-left: 80px;
border-radius: 30px;
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
  text-decoration: none;
}
</style>