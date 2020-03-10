<template>
  <div id="app">
    <Grid />
  </div>
</template>

<script>
import Grid from './components/Grid.vue'

export default {
  name: 'App',
  components: {
    Grid
  }
}
</script>

<style>
 @import url('https://fonts.googleapis.com/css?family=Roboto:100,300,400,500,700,900&display=swap');

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Roboto;
  }
 body {
    display: flex;
    justify-content: center;
    align-self: center;
    min-height: 100vh;
    background: #637bff;
  }
  #app {
    width: 100%;
    height: 100%;
  }
</style>
