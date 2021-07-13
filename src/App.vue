<template>
  <div id="app">
    <HelloWorld v-show="false"/>
    <DirectivasExample/>
    <DirectivasBindAndModel/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import DirectivasExample from './components/DirectivasExample.vue'
import DirectivasBindAndModel from './components/DirectivasBindAndModel.vue'


export default {
  name: 'App',
  components: {
    HelloWorld,
    DirectivasExample,
    DirectivasBindAndModel
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
