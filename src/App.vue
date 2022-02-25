<template>
  <div id="main">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>{{title}}</h1>
    <!-- <button @click="title = 'DRUGI NAZIV'">change title</button> -->
    
    <!-- obicno sabiranje/oduzimanje-->
    <p>Number = number + 1</p>
    <button @click="number1 = number1 + 1">+</button>
    <h3>{{number1}}</h3>
    <button @click="number1 = number1 - 1">-</button> 

<!---->
    <p>Number = number ++</p>
    <button @click="number2++">+</button>
    <h3>{{number2}}</h3>
    <button @click="number2--">-</button>

  </div>
</template>

<script>
export default {
data() {
  return {
    title:'VUE OBUKA',
    number1: 0,
    number2: 0
  }
},
}
</script>

<style>
#main {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
