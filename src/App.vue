<template>
  <div id="app">
    <h1>Calculadora</h1>
    <Calculator @onError="onError"/>
  </div>
</template>

<script>
import Calculator from './Calculator'

export default {
  components: { Calculator },
  methods: {
    onError() {
      alert('Erro!')
    }
  }
}
</script>

<style>
@font-face {
  font-family: 'RobotoMono';
  src: url('./fonts/RobotoMono-Thin.ttf');
}

* {
  font-family: 'RobotoMono', monospace;
}

body {
  margin: 0;
}

#app {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
}
</style>