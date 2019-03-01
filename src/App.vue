<template>
  <div id="app">
    <img src="./assets/logo.png">
    <btn-bar :barLen="5"
             :barList="list"></btn-bar>
    <!--<router-view/>-->
  </div>
</template>

<script>
import BtnBar from '../src/components/basic-ui/btnlike-bar/btn-frame'
export default {
  name: 'App',
  components: {
    BtnBar
  },
  data () {
    return {
      list: []
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
