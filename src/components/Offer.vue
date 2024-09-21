<template>
    <section class="Offer" id="Offer">
      <div class="text">
        <h1>Offer</h1>
        <h2>仕事依頼</h2>
      </div>
    </section>
    </template>
      
    <script>
    export default {
      name: 'NiceOffer'
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
    </style>