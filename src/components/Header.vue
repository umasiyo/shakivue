<template>
  <div class="header">
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

<!-- Add "scoped" attribute to limit CSS to this component only -->
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
  line-height:70px;
  text-align:center;
}
.menu li{
  list-style: none;
  float:left;
  color: white;
}

</style>
