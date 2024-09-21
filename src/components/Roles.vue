<template>
<section class="roles" id="Roles">
  <div class="contents">
    <h1>Roles</h1>
    <h2>役割について</h2>
    <div class="zukei">
      <ul class="list">
        <li>
          <input type="radio" name="setumei" id="btn01" class="radio" checked>
          <label for="btn01" class="btn">first</label>
          <div class="first_setumei">
            <p>3Dモデリング、プログラム<br>もっと写真増やしたい<br>上の丸の部分にパット見のイラストがほしい<br>素材できたらください</p>
            <img src="../assets/03c889d160a2fe1eb248e7772eafe81a.jpg" />
          </div>
        </li>
        <li>
          <input type="radio" name="setumei" id="btn02" class="radio">
          <label for="btn02" class="btn">second</label>
          <div class="second_setumei">
            <p>構成、編集</p>
            <img src="../assets/mukashiekonte.png" />
          </div>
        </li>
        <li>
          <input type="radio" name="setumei" id="btn03" class="radio">
          <label for="btn03" class="btn">third</label>
          <div class="third_setumei">
            <p>撮影</p>
            <img src="../assets/countdownhirata_seisakukatei.png" />
          </div>
        </li>
        <li>
          <input type="radio" name="setumei" id="btn04" class="radio">
          <label for="btn04" class="btn">fourth</label>
          <div class="fourth_setumei">
            <p>業務管理</p>
            <img src="../assets/countdownhirata_seisakukatei.png" />
          </div>
        </li>
      </ul>
    </div>
    <div class="btns">
      <a class="button insta" href="https://www.instagram.com/shakilstudio.temp/" target="_blank" rel="noopener">質問等はこちらのDMまで!</a>
      <a class="button googleform" href="https://forms.gle/KLi59rPmnbTE9RGG8" target="_blank" rel="noopener">参加したい方はここから!</a>
    </div>
  </div>
</section>
</template>
  
<script>
export default {
  name: 'NiceRoles'
}
</script>

<style scoped>
section {
  width: 100%;
  height: 700px;
  position: relative;
}
.contents {
  width: 50%;
  position: absolute;
  left: 18%;
  margin: 0;
  padding: 0;
}
.contents h1 {
  font-size: 3rem;
  margin-bottom: 0;
  color: #CC8800;
}
.contents h2 {
  font-size: 1.8rem;
  margin-top: 0;
}
.zukei {
  display: flex;
}
.list {
  position: relative;
  display: flex;
}
.roles li {
  list-style: none;
  width: 70px;
  height: 70px;
  margin-right: 2rem;
}
.radio {
	display: none;
}
/*tuika*/
.btn {
	display: flex;
	align-items: center;
	justify-content: center;
	width: 70px;
  height: 70px;
  background: #d9d9d9;
	border-radius:50%;
	font-size: 1.0rem;
	cursor: pointer;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
}
.first_setumei {
  width: 200%;
  height: 20rem;
  position: absolute;
  top: 0%;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  display: none;
  translate: 0 30%;
}
.first_setumei p {
  width: 40%;
  float: left;
}
.first_setumei img {
  width: 50%;
  height: 20rem;
  float: left;
  object-fit: cover;
}
.second_setumei {
  width: 200%;
  height: 20rem;
  position: absolute;
  top: 0%;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  display: none;
  translate: 0 30%;
}
.second_setumei p {
  width: 40%;
  float: left;
}
.second_setumei img {
  height: 20rem;
  float: left;
  object-fit: cover;
}
.third_setumei {
  width: 200%;
  height: 20rem;
  position: absolute;
  top: 0%;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  display: none;
  translate: 0 30%;
}
.third_setumei p {
  width: 40%;
  float: left;
}
.third_setumei img {
  width: 50%;
  height: 20rem;
  float: left;
  object-fit: cover;
}
.fourth_setumei {
  width: 200%;
  height: 20rem;
  position: absolute;
  top: 0%;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  display: none;
  translate: 0 30%;
}
.fourth_setumei p {
  width: 40%;
  float: left;
}
.fourth_setumei img {
  width: 50%;
  height: 20rem;
  float: left;
  object-fit: cover;
}
.radio:checked+.btn {
  border: solid 2px;
  border-color: #1ad33a;
}
.radio:checked~.first_setumei {
  display: block;
}
.radio:checked~.second_setumei {
  display: block;
}
.radio:checked~.third_setumei {
  display: block;
}
.radio:checked~.fourth_setumei {
  display: block;
}
/*tuika*/
.contents div {
  clear: both;
}
.btns {
  translate: 0 900%;
}
.button {
  font-size: 1.5rem;
  font-weight: 600;
  line-height: 40px;
  text-align: center;
  border-radius: 20px;
  width: 450px;
  height: 40px;
  text-decoration: none;
  padding:5px 25px;
  margin-right: 50px;
}
.insta {
  background: white;
  color: black;
  border: solid 2px;
  border-color: #082B71;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
}
.googleform {
  background: linear-gradient(to right, #E85BFF, #03F0FF);
  color: white;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
}

</style>