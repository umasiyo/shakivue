<template>
    <html lang="ja">
      <head>
        <meta charset="UTF-8">
      </head>
  
      <body>
        <main class="About">
          <h1>About</h1>
        </main>
      </body>
    </html>
  </template>
  
  <script>
  export default {
    name: 'NiceAbout'
  }
  </script>
  
  <!-- ここでのCSSはこのcomponentでしか使用できない -->
  <style scoped>
  /* *{border:solid 1px red;} */
  
  html{ font-size: 100%; }
  body{ margin: 0; padding: 0;}
  </style>