<template>
<section class="works" id="Works">
  <div class="text">
    <h1>Works</h1>
    <h2>作成した作品の一部</h2>
  </div>
  <div class="scroll-infinity">
    <div class="scroll-infinity__wrap">
      <ul class="scroll-infinity__list scroll-infinity__list--left">
        <li class="scroll-infinity__item">
          <img src="../assets/testpic_1.png" />
          <h3>作品名1</h3>
          <p>説明文1</p>
        </li>
        <li class="scroll-infinity__item">
          <img src="../assets/testpic_2.png" />
          <h3>作品名2</h3>
          <p>説明文2</p>
        </li>
        <li class="scroll-infinity__item">
          <img src="../assets/testpic_1.png" />
          <h3>作品名1</h3>
          <p>説明文1</p>
        </li>
        <li class="scroll-infinity__item">
          <img src="../assets/testpic_2.png" />
          <h3>作品名2</h3>
          <p>説明文2</p>
        </li>
      </ul>
      <ul class="scroll-infinity__list scroll-infinity__list--left">
        <li class="scroll-infinity__item">
          <img src="../assets/testpic_1.png" />
          <h3>作品名1</h3>
          <p>説明文1</p>
        </li>                        
        <li class="scroll-infinity__item">
          <img src="../assets/testpic_2.png" />
          <h3>作品名2</h3>
          <p>説明文2</p>
        </li>
        <li class="scroll-infinity__item">
          <img src="../assets/testpic_1.png" />
          <h3>作品名1</h3>
          <p>説明文1</p>
        </li>
        <li class="scroll-infinity__item">
          <img src="../assets/testpic_2.png" />
          <h3>作品名2</h3>
          <p>説明文2</p>
        </li>
      </ul>
    </div>
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
  color: #102246;
  margin-bottom: 0;
}
.text h2 {
  font-size: 1.8rem;
  color: #5077C5;
  margin-top: 0;
}

.scroll-infinity {
  position: absolute;
  top: 30%;
}

@keyframes infinity-scroll-left {
from {
  transform: translateX(0);
}
  to {
  transform: translateX(-100%);
}
}
.scroll-infinity__wrap {
  display: flex;
  overflow: hidden;
}
.scroll-infinity__list {
  display: flex;
  list-style: none;
  padding: 0
}
.scroll-infinity__list--left {
  animation: infinity-scroll-left 80s infinite linear 0.5s both;
}
.scroll-infinity__item {
  width: calc(100vw / 4);
  margin: 0 2rem;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
}
.scroll-infinity__item>img {
  width: 100%;
}
</style>