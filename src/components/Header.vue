<template>
<a href="#Top">
<header class="wrapper">
  <div class="shakilstudio">
    <a href="https://umasiyo.github.io/shakivue/">
      <img src="../assets/logo_white.png" alt="ShakilStudio_logo" class="logo">
      <h1>SHAKIL STUDIO</h1>
    </a>
  </div>
  <div>
    <nav>
      <ul class="nav">
        <li><a href="#About">ABOUT</a></li>
        <li><a href="#Works">WORKS</a></li>
        <li><a href="#Records">RECORDS</a></li>
        <li><a href="#Form">FORM</a></li>
      </ul>
    </nav>
  </div>
  <div class="insta_logo">
    <a href="https://www.instagram.com/shakilstudio.temp/" target="_blank" rel="noopener">
      <img src="../assets/ig_logo.png" alt="Instagram_logo" class="logo">
    </a>
  </div>
</header>
</a>
</template>

<script>
export default {
  name: 'NiceHeader',
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
header{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 70px;
  z-index: 10;
  background-color: #082B71;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.shakilstudio a{ display: flex; align-items: center; }
.shakilstudio h1{ float: right; color: white; }
.nav{ display: flex; font-size: 20px; text-transform: uppercase; font-weight: 200; align-items: center; list-style: none; }/*min10px,max23px*//*font-family: Montserrat;*/
.nav li{margin-left: 14px; }
.nav a{ color: white; text-decoration: none;}
img.logo { width: 37px; height: 37px; padding: 15px; }
</style>