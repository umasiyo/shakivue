<template>
  <div class="header">
    <ul>
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
  width:1280px;
  height:60px;
  background-color: #082B71;
}
</style>
