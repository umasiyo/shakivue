<template>
  <NiceHeader/>
  <NiceTop/>
  <NiceAbout/>
  <NiceWorks/>
  <NiceRecords/>
  <NiceForm/>
  <NiceFooter/>
  <!-- <HelloWorld/> -->
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import NiceHeader from './components/Header.vue'
import NiceTop from './components/Top.vue'
import NiceAbout from './components/About.vue'
import NiceWorks from './components/Works.vue'
import NiceRecords from './components/Records.vue'
import NiceForm from './components/Form.vue'
import NiceFooter from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    NiceHeader,
    NiceTop,
    NiceAbout,
    NiceWorks,
    NiceRecords,
    NiceForm,
    NiceFooter
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
