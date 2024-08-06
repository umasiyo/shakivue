<template>
<section class="form" id="Form">
  <div class="contents">
    <h1>Form</h1>
    <h2>参加したい？歓迎するよ！</h2>
    <ul class="zukei list">
      <li></li>
      <li></li>
      <li></li>
      <li></li>
    </ul>
    <p class="zukei setumei"></p>
    <div class="Buttons">
      <a class="button insta" href="https://www.instagram.com/shakilstudio.temp/" target="_blank" rel="noopener">質問等はこちらのDMまで!</a>
      <a class="button googleform" href="https://forms.gle/KLi59rPmnbTE9RGG8" target="_blank" rel="noopener">お申し込みはここから!</a>
    </div>
  </div>
  <img src="../assets/hiratasan.png" alt="hiratasan" class="hiratasan">
</section>
</template>
  
<script>
export default {
  name: 'NiceForm'
}
</script>

<style scoped>
section{ width: 100%; height: 700px; background-color: white; }
.contents{ width: 80%; position: relative; top: 15%; left: 18%; margin: 0; padding: 0;}
.contents h1{ font-size: 60px; color: black; margin-bottom: 0; }
.contents h2{ font-size: 30px; color: #314F87; margin-top: 0; }
.zukei{position: relative; left:5%;}
.form ul{list-style: none;}
.form li{background-color: #d9d9d9; width: 70px; height: 70px; border-radius: 50%; margin-bottom: 10px;}
.list{ float: left;}
.setumei{ float: left; width: 600px; height: 320px; background-color: #d9d9d9; list-style: none; margin-left: 80px; border-radius: 30px; }
.Buttons{clear: both;position: relative; left:5%;}
.button{
  font-size: 20px;
  font-weight: 600;
  line-height: 40px;
  text-align: center;
  border-radius: 20px;
  width: 450px;
  height: 40px;
  text-decoration: none;
  padding:5px 25px;
  margin-right: 50px;
}
.insta{background-color: white; color: black; border: solid 2px; border-color: #082B71;}
.googleform{background: linear-gradient(to right, #E85BFF, #03F0FF); color: white;}
.hiratasan{ position: relative; top: -300px; left: 65%;}
</style>