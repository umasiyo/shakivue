<template>
<section class="Records" id="Records">
  <div class="text">
    <h1>Records</h1>
    <h2>どんな生活を送っているのか？</h2>
  </div>
</section>
</template>
  
<script>
export default {
  name: 'NiceRecords'
}
</script>

<style scoped>
section {
  width: 100%;
  height: 600px;
  background: rgb(153, 51, 51);
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