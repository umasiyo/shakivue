<template>
  <div class="header">
    <img alt="Shak_logo" src="../assets/logo_white.png">
    <ul class="menu">
      <li><a href="https://vuejs.org" target="_blank" rel="noopener">ABOUT</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">WORKS</a></li>
      <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">RECORDS</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">FORM</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'NiceHeader',
  props: {
    msg: String
  }
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
.header{
  width:100%;
  height:70px;
  background-color: #082B71;
  position:fixed;
  top:0;
  left:0;
  z-index:10;
}
.menu{
  display: flex;
  justify-content: center;
}

.menu li{
  list-style: none;
  float:left;
  color: white;
  padding: 10px;
}
.menu a{
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  color: white;
  text-decoration: none;
}

</style>
