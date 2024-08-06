<template>
<section class="ｗorks" id="Works">
  <div class="text">
    <h1>Works</h1>
    <h2>たとえば何作ってんすか？</h2>
  </div>
</section>
</template>
  
<script>
export default {
  name: 'NiceWorks'
}
</script>

<style scoped>
section{
  width: 100%;
  height: 600px;
  background: rgb(143, 125, 125);
  position: relative;
}
.text {
  width: 50%;
  text-align: left;
  position: absolute;
  top: 5%;
  left: 18%;
  margin: 0;
  padding: 0;
}
.text h1 {
  font-size: 3rem;
  color: black;
  margin-bottom: 0;
}
.text h2 {
  font-size: 1.8rem;
  color: #314F87;
  margin-top: 0;
}
</style>