<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />

    <vue-loop :full="true" :horizontal="false" id="autoscroll">
      <div class="item">1 das</div>
      <div class="item">2 ist noch nicht</div>
      <div class="item">3 ganz das</div>
      <div class="item">4 was ich will</div>
    </vue-loop>
  </div>
</template>

<script>
  import VueLoop from 'vue-loop'

  export default {
    name: 'App',
    components: {
      VueLoop,
    },
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
  .item {
    font-size: 40px;
  }

  /* #autoscroll {
    animation: slide infinite 2s normal linear;
  } */

  @keyframes slide {
    0% {
      margin-top: 100vh;
    }
    100% {
      margin-top: -000vh;
    }
  }
</style>
