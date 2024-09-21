<template>
<section class="records" id="Records">
  <div class="text">
    <h1>Records</h1>
    <h2>詳細な活動内容</h2>
  </div>
  <div class="record1">
    <div class="record1box">撮影風景写真</div>
    <div class="record1circle">
      <p>ポスターや動画作成の際に<br>素材が必要になった場合は,<br>自分たちで撮影を行います。</p>
    </div>
  </div>
  <div class="record2">
    <div class="record2box">discordのやりとり、会議の写真</div>
    <div class="record2circle">
      <p>普段はDiscord上で会議を行い<br>個々がやりたいことに合わせて<br>役割、タスクの決定をします。<br>制作物の意見交換など<br>積極的に行っています。</p>
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
  margin-bottom: 0;
  color: #CC8800;
}
.text h2 {
  font-size: 1.8rem;
  margin-top: 0;
}
.record1 {
  width: 50%;
  height: 350px;
  position: absolute;
  top: 30%;
  left: 0;
}
.record1box {
  width: 240px;
  height: 240px;
  position: absolute;
  top: 15%;
  left: 50%;
  background: #D9D9D9;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
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
  background: #252525;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  transition: all 1s;
  z-index: 1;
}
.record1circle p {
  text-align: center;
  position: relative;
  top: 30%;
}
.record2 {
  width: 50%;
  height: 350px;
  position: absolute;
  top: 30%;
  left: 50%;
}
.record2box {
  width: 240px;
  height: 240px;
  position: absolute;
  top: 15%;
  left: 14%;
  background: #D9D9D9;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
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
  background: #252525;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  transition: all 1.2s;
  z-index: 1;
}
.record2circle p {
  text-align: center;
  position: relative;
  top: 25%;
}
.record1:hover .record1box{
  left:36%;
}
.record1:hover .record1circle{
  left:68%;
}
.record2:hover .record2box{
  left:0%;
}
.record2:hover .record2circle{
  left:32%;
}

</style>