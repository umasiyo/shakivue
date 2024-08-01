<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <NiceHeader/>
  <HelloWorld/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import NiceHeader from './components/Header.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    NiceHeader
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
