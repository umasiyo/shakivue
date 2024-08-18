<template>
<section class="form" id="Form">
  <div class="contents">
    <h1>Form</h1>
    <h2>参加したい？歓迎するよ！</h2>
    <div class="zukei">
      <ul class="list">
        <li></li>
        <li></li>
        <li></li>
        <li></li>
      </ul>
      <p class="setumei"></p>
    </div>
    <div>
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
section {
  width: 100%;
  height: 700px;
  background: rgb(160, 124, 124);
  position: relative;
}
.contents {
  width: 50%;
  position: absolute;
  top: 5%;
  left: 18%;
  margin: 0;
  padding: 0;
}
.contents h1 {
  font-size: 3rem;
  color: black;
  margin-bottom: 0;
}
.contents h2 {
  font-size: 1.8rem;
  color: #314F87;
  margin-top: 0;
}
.zukei {
  display: flex;
}
.form li {
  list-style: none;
  background: #d9d9d9;
  width: 70px;
  height: 70px;
  border-radius: 50%;
  margin-bottom: 10px;
}
.setumei {
  width: 600px;
  height: 320px;
  background-color: #d9d9d9;
  margin-left: 80px;
  border-radius: 30px;
}
.contents div {
  clear: both;
}
.button {
  font-size: 1.5rem;
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
.insta {
  background: white;
  color: black;
  border: solid 2px;
  border-color: #082B71;
}
.googleform {
  background: linear-gradient(to right, #E85BFF, #03F0FF);
  color: white;
}
.hiratasan {
  position: absolute;
  top: 25%;
  left: 65%;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
}
</style>