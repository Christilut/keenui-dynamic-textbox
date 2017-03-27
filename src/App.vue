<template>
  <div id="app">
    <img src="./assets/logo.png">
    <hello></hello>
    <ui-textbox v-model="newContent['textbox']" placeholder="Textbox"></ui-textbox>
  </div>
</template>

<script>
import Hello from './components/Hello'

export default {
  name: 'app',
  components: {
    Hello
  },
  data () {
    return {
      newContent: {}
    }
  },
  created () {
    this.newContent['textbox'] = 'test'
  }
}
</script>

<style lang="scss">
@import '../node_modules/keen-ui/dist/keen-ui.min';
</style>

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
