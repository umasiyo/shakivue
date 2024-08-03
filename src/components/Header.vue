<template>
  <html lang="ja">
    <head>
      <meta charset="UTF-8">
      <title>シャキルスタジオメンバー募集</title>
      <meta name="description" content="シャキルスタジオ（仮）の再始動に際し、新たなメンバーを募集する。">
    </head>

    <body>
      <div class="header">
        <div>
          <a href="https://umasiyo.github.io/shakivue/">
            <img src="../assets/logo_white.png" alt="ShakilStudio_logo" class="logo">
          </a>
        </div>
        <div><ul class="menu">
          <li><a href="https://vuejs.org" target="_blank" rel="noopener">ABOUT</a></li>
          <li><a href="https://forum.vuejs.org" target="_blank" rel="noopener">WORKS</a></li>
          <li><a href="https://chat.vuejs.org" target="_blank" rel="noopener">RECORDS</a></li>
          <li><a href="https://twitter.com/vuejs" target="_blank" rel="noopener">FORM</a></li>
        </ul></div>
        <div>
          <a href="https://www.instagram.com/">
            <img src="../assets/ig_logo.png" alt="Instagram_logo" class="logo">
          </a>
        </div>
      </div>
    </body>
  </html>
</template>

<script>
export default {
  name: 'NiceHeader',
}
</script>

<!-- ここでのCSSはこのcomponentでしか使用できない -->
<style scoped>
html{
  font-size: 100%;
}

.header{
  position: fixed;
  top: 0;
  left: 0;
  margin: 0;
  z-index: 10;
  width: 100lvw;
  height: 70px;
  background-color: #082B71;
  display: flex;
  justify-content: space-between;
}

.menu li{
  margin: 0;
  height: 70px;
  padding: 0 10px;
  float: left;
  list-style: none;
}

.menu a{
  font-family: Montserrat;
  font-weight: bolder;
  font-size: clamp(0.625rem, 0.33rem + 1.48vw, 1.438rem);/*min10px,max23px*/
  color: white;
  text-decoration: none;
}

img.logo {
  width: 37px;
  height: 37px;
  padding: 15px;
}

</style>
