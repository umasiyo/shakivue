<template>
<footer>
  <div class="right"><!--右端揃えるやつら-->
    <nav>
      <ul class="nav">
        <li><a href="#About">ABOUT</a></li>
        <li><a href="#Works">WORKS</a></li>
        <li><a href="#Records">RECORDS</a></li>
        <li><a href="#Form">FORM</a></li>
      </ul>
    </nav>
    <h3>CONTACT US</h3>
    <a class="insta" href="https://www.instagram.com/shakilstudio.temp/" target="_blank" rel="noopener">IG @shakilstudio</a><!--ここリンク出てこないのまじで治らないので見て見ぬふりしてます-->
  </div>
  <div class="left"><!--左端揃えるやつら-->
      <p><small>&copy; 2024 Shakil Studio. All rights reserved.</small></p>
      <div class="shakilstudio">
        <img src="../assets/logo_white.png" alt="ShakilStudio_logo" class="logo">
        <img src="../assets/textlogo_white.png" alt="ShakilStudio_textlogo" class="textlogo">
    </div>
  </div>
</footer>
</template>
  
<script>
export default {
  name: 'NiceFooter'
}
</script>

<style scoped>
footer {
  width: 100%;
  height: 420px;
  position: relative;
}
.right {
  text-align: right;
  position: absolute;
  top: 10%;
  right: 18%;
}
.nav {
  font-size: 1.5rem;
  font-weight: 200;
  list-style: none;
}
.nav li {
  margin-bottom: 8px;
}
.nav a{
  color: white;
  text-decoration: none;
  transition: 0.2s;
}
.nav a:hover {
  color: rgba(255, 255, 255, 0.567);
}
footer h3{
  font-size: 1.5rem;
  font-weight: 600;
  margin-bottom: 25px;
}
.insta {
  clear: both;
  font-size: 23px;
  color: white;
  text-decoration: none;
  font-weight: 200;
}
.left {
  width: 50%;
  height:0;
  text-align: left;
  position: absolute;
  top: 60%;
  left: 18%;
}/*width80%にしてたとき、rightのinstaテキストと被ってリンク飛べなかったので、他の要素と被らないように注意*/
.shakilstudio {
  display: flex;
  align-items: center;
}
.left p {
  margin-bottom: 0;
}
.shakilstudio h1 {
  float: right;
  font-size: 4rem;
  font-weight: 600;
  margin: 0;
}
.logo {
  width: 70px;
  height: 70px;
  padding-right: 30px;
  margin: 0;
}
.textlogo {
  width: 520px;
  height: 60px;
  margin: 0;
}/*シャキスタロゴ、インスタロゴのサイズ設定*/
</style>