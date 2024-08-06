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
        <h1>SHAKIL STUDIO</h1>
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
footer{ background-color: #082B71; width: 100%; height: 420px; color: white; }
.right { text-align: right; position: relative; top: 10%; right: 18%; }
.nav{
  font-size: 23px;
  text-transform: uppercase;
  font-weight: 200;
  list-style: none;
}
.nav li{ margin-bottom: 8px; }
.nav a{ color: white; text-decoration: none; }
footer h3{ font-size: 23px; text-transform: uppercase; font-weight: 600; }
.left p{ margin-bottom: 0;}
.insta{ clear: both; font-size: 23px; color: white; text-decoration: none; font-weight: 200; }
.text h1{font-size: 60px; color: black; margin-bottom: 0}
.left { width: 50%; height:0; text-align: left; position: relative; top: 3%; left: 18%;}/*width80%にしてたとき、rightのinstaテキストと被ってリンク飛べなかったので、他の要素と被らないように注意*/
.shakilstudio{ display: flex; align-items: center; position: relative; top: -30px;}
.shakilstudio h1{ float: right; font-size: 60px; font-weight: 600; }
img.logo{ width: 80px; height: 80px; padding-right: 20px; }
</style>