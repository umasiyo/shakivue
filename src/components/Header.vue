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
html{
  font-size: 100%;
}

.header{
  position: fixed;
  top: 0;
  left: 0;
  margin: 0;
  z-index: 10;
  width: 100lvw;
  height: 70px;
  background-color: #082B71;
  display: flex;
  justify-content: space-between;
}

menu {
  display: flex;
  align-items: center;
}

.menu li{
  list-style: none;
  float: left;
  padding: 0 10px;
}

.menu a{
  font-family: Montserrat;
  font-weight: bolder;
  font-size: clamp(0.625rem, 0.33rem + 1.48vw, 1.438rem);/*min10px,max23px*/
  line-height: 70px;
  color: white;
  text-decoration: none;
}

img.logo {
  width: 37px;
  height: 37px;
  padding: 15px;
}

</style>
