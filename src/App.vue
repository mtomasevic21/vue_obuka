<template>
  <div id="main">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>{{title}}</h1>
    
    <button @click="addNumber()">+</button>
    <h3>{{number1}}</h3>
    <button @click="removeNumber()">-</button> 

  </div>
</template>
<!-- ovde pisemo promenljive, stringovi, brojevi, nizovi i objekti-->
<script>
export default {
data() {
  return {
    title:'VUE OBUKA',
    number1: 0,
    number2: 0

  }
},

methods:{
  addNumber(){
    this.number1 = this.number1 + 1
  },
  removeNumber(){
    this.number1 = this.number1 - 1
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
