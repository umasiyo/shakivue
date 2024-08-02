<template>
  <div class="header">
    <div>
    <img alt="Shak_logo" src="../assets/logo_white.png" class="logo">
    </div>
    <div><ul class="menu">
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">ABOUT</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">WORKS</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">RECORDS</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">FORM</a></li>
    </ul></div>
    <div><img src="../assets/ig_logo.png" alt="Instagram_logo" class="logo"></div>
  </div>
</template>

<script>
export default {
  name: 'NiceHeader',
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
.header{
  width: 100%;
  height: 70px;
  background-color: #082B71;
  position: fixed;
  top: 0;
  left: 0;
  z-index: 10;
  display: flex;
  justify-content: space-between;
}

.menu li{
  list-style: none;
  float: left;
  color: white;
  padding: 10px;
}

.menu a{
  font-family: Montserrat;
  font-weight: bolder;
  font-size: clamp(1.25rem, 1.136rem + 0.57vw, 1.563rem);
  color: white;
  text-decoration: none;
}

img.logo {
  width: 37px;
  height: 37px;
  padding: 15px;
}

</style>
