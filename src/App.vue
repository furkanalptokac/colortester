<template>
  <div id="app">
  <h2>Test a color.</h2>
  <input type="text"  v-model="color" maxlength="7" placeholder="#000000">
  Color Picker: <input type="color" v-model="color">
    <div id="color" v-bind:style="{backgroundColor: color}"/>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      color: '#ff9000'
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
}

#color {
  width: 500px;
  height: 500px;
  margin: 0 auto;
  margin-top: 20px;
}

h1, h2 {
  font-weight: normal;
}
</style>
