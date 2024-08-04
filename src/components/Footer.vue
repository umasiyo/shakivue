<template>
  <footer>
    <div class="right">
      <div>
        <nav>
          <ul class="nav">
            <li><a href="https://vuejs.org" target="_blank" rel="noopener">ABOUT</a></li>
            <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">WORKS</a></li>
            <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">RECORDS</a></li>
            <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">FORM</a></li>
          </ul>
        </nav>
        <h3>CONTACT US</h3>
        <a href="https://www.instagram.com/" target="_blank" rel="noopener"><h4>IG @shakilstudio</h4></a>
      </div>
    </div>
    <div class="left">
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

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
/* *{border:solid 1px red;} */
footer{ background: #082B71; width: 100%; height: 420px; color: white; }
.right { text-align: right; position: relative; top: 50px; right: 18%; }
.nav{
  font-size: 23px;
  text-transform: uppercase;
  font-weight: 200;
  list-style: none;
}
/*min10px,max23px*//*font-family: Montserrat;*/
.nav li{ margin-bottom: 8px; }
.nav a{ color: white; text-decoration: none; }
footer h3{ font-size: 23px; text-transform: uppercase; font-weight: 600; }
.right a{ font-size: 23px; color: white; text-decoration: none; font-weight: 200; }
.left{ text-align: left; position: relative; top: -30px; left: 18%; }
.shakilstudio{ display: flex; align-items: center; position: relative; top: -50px; }
.shakilstudio h1{ float: right; font-size: 60px; font-weight: 600; }
img.logo{ width: 80px; height: 80px; padding-right: 20px; }
</style>