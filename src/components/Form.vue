<template>
<section class="form" id="Form">
  <div class="contents">
    <h1>Form</h1>
    <h2>参加したい？歓迎するよ！</h2>
    <div class="zukei">
      <ul class="list">
        <li>
          <input type="radio" name="setumei" id="btn01" class="radio" checked>
          <label for="btn01" class="btn">first</label>
          <div class="first_setumei">1つ目の説明を記入</div>
        </li>
        <li>
          <input type="radio" name="setumei" id="btn02" class="radio">
          <label for="btn02" class="btn">second</label>
          <div class="second_setumei">2つ目の説明を記入</div>
        </li>
        <li>
          <input type="radio" name="setumei" id="btn03" class="radio">
          <label for="btn03" class="btn">third</label>
          <div class="third_setumei">3つ目の説明を記入</div>
        </li>
        <li>
          <input type="radio" name="setumei" id="btn04" class="radio">
          <label for="btn04" class="btn">fourth</label>
          <div class="fourth_setumei">4つ目の説明を記入</div>
        </li>
      </ul>
    </div>
    <div>
      <a class="button insta" href="https://www.instagram.com/shakilstudio.temp/" target="_blank" rel="noopener">質問等はこちらのDMまで!</a>
      <a class="button googleform" href="https://forms.gle/KLi59rPmnbTE9RGG8" target="_blank" rel="noopener">お申し込みはここから!</a>
    </div>
  </div>
  <img src="../assets/hiratasan.png" alt="hiratasan" class="hiratasan">
</section>
</template>
  
<script>
export default {
  name: 'NiceForm'
}
</script>

<style scoped>
section {
  width: 100%;
  height: 700px;
  background: white;
  position: relative;
}
.contents {
  width: 50%;
  position: absolute;
  top: 5%;
  left: 18%;
  margin: 0;
  padding: 0;
}
.contents h1 {
  font-size: 3rem;
  color: black;
  margin-bottom: 0;
}
.contents h2 {
  font-size: 1.8rem;
  color: #314F87;
  margin-top: 0;
}
.zukei {
  display: flex;
}
.form li {
  list-style: none;
  width: 70px;
  height: 70px;
  margin-bottom: 10px;
}
/*tuika*/
.btn {
	display: flex;
	align-items: center;
	justify-content: center;
	width: 70px;
  height: 70px;
  background: #d9d9d9;
	color: #fff;
	border-radius:50%;
	font-size: 1.0rem;
	cursor: pointer;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
}
.radio {
	display: none;
}
.list {
  position: relative;
}
.first_setumei {
  width: 600px;
  height: 320px;
  position: absolute;
  top: 0%;
  left: 50%;
  background-color: yellow;
  margin-left: 80px;
  border-radius: 30px;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  display: none;
}
.second_setumei {
  width: 600px;
  height: 320px;
  position: absolute;
  top: 0%;
  left: 50%;
  background-color: red;
  margin-left: 80px;
  border-radius: 30px;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  display: none;
}
.third_setumei {
  width: 600px;
  height: 320px;
  position: absolute;
  top: 0%;
  left: 50%;
  background-color: blue;
  margin-left: 80px;
  border-radius: 30px;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  display: none;
}
.fourth_setumei {
  width: 600px;
  height: 320px;
  position: absolute;
  top: 0%;
  left: 50%;
  background-color: green;
  margin-left: 80px;
  border-radius: 30px;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
  display: none;
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
.hiratasan {
  position: absolute;
  top: 25%;
  left: 65%;
  filter: drop-shadow(0px 0px 2px #4f4e4e);
}
</style>