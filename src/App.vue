<template>
  <div id="app">
    <Contador/>
  </div>
</template>

<script>
import Contador from './components/Contador'

export default {
  name: 'App',
  components: {
    Contador
  }
}
</script>

<style>
  /*#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }*/
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body{
    width: 100vw;
    min-height: 100vh;
    font-family: Tahoma;
    font-size: 18px;
  }
</style>
