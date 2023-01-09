<template>
  <div id="container" v-bind:style="{backgroundColor: color}">
    <h1>Cambiar el color</h1>
    <div class="row">
      <div class="col-md-4"></div>
      <div class="col-md-4">
        <input type="text" class="form-control mb-3" v-bind:style="{ color: color}" v-model="color" placeholder="#000000"/>
        <input type="color" v-model="color"/>
      </div>
      <div class="col-md-4"></div>
    </div>

  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data () {
    return {
      color: '#674DB9'
    }
  },
  components: {
    //HelloWorld
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
}
h1 {
  color: #ffffff;
}
#container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: center;
}
</style>
