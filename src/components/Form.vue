<template>
<section class="form" id="Form">
  <div class="text">
    <h1>Form</h1>
    <h2>参加したい？歓迎するよ！</h2>
  </div>
</section>
</template>
  
<script>
export default {
  name: 'NiceForm'
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
/* *{border:solid 1px red;} */
section{ width: 100%; height: 600px; background-color: white; }
.text{ width: 80%; text-align: left; position: relative; top: 15%; left: 18%; margin: 0; padding: 0;}
.text h1{ font-size: 60px; color: black; margin-bottom: 0; }
.text h2{ font-size: 30px; color: #314F87; margin-top: 0; }
</style>