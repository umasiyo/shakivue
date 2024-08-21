<template>
<section class="Records" id="Records">
  <div class="text">
    <h1>Records</h1>
    <h2>どんな生活を送っているのか？</h2>
  </div>
  <div class="record1">
    <div class="record1box"></div>
    <div class="record1circle">
      <p>aaa</p>
    </div>
  </div>
  <div class="record2">
    <div class="record2box"></div>
    <div class="record2circle">
      <p>bbb</p>
    </div>
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
  background: white;
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
.record1 {
  width: 50%;
  height: 350px;
  position: absolute;
  top: 30%;
  left: 0;
  background: white;
}
.record1box {
  width: 240px;
  height: 240px;
  position: absolute;
  top: 15%;
  left: 50%;
  background: #252525;
  transition: all 1s;
  z-index: 2;
}
.record1circle {
  width: 240px;
  height: 240px;
  border-radius: 50%;
  position: absolute;
  top: 15%;
  left: 55%;
  background: #D9D9D9;
  transition: all 1s;
  z-index: 1;
}
.record1circle p {
  position: absolute;
  top: 40%;
}
.record2 {
  width: 50%;
  height: 350px;
  position: absolute;
  top: 30%;
  left: 50%;
  background: white;
}
.record2box {
  width: 240px;
  height: 240px;
  position: absolute;
  top: 15%;
  left: 14%;
  background: #252525;
  transition: all 1.2s;
  z-index: 2;
}
.record2circle {
  width: 240px;
  height: 240px;
  border-radius: 50%;
  position: absolute;
  top: 15%;
  left: 19%;
  background: #D9D9D9;
  transition: all 1.2s;
  z-index: 1;
}
.record2circle p {
  position: absolute;
  top: 40%;
}
@keyframes rotate_circle {
    0% {
        transform:rotate(0deg);/* アニメーションの進みが0%の時の状態 */
    }
    100% {
        transform:rotate(360deg);/* アニメーションの進みが100%の時の状態 */
    }
}
.record1:hover .record1box{
  left:36%;
}
.record1:hover .record1circle{
  left:68%;
  animation: rotate_circle 5s;
}
.record2:hover .record2box{
  left:0%;
}
.record2:hover .record2circle{
  left:32%;
  animation: rotate_circle 5s;
}
</style>