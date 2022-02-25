<template>
  <div id="main">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>{{title}}</h1>
    
    <button @click="changeNumber('plus')">+</button>
    <h3>{{number}}</h3>
    <button @click="changeNumber('minus')">-</button> 

  </div>
</template>
<!-- ovde pisemo promenljive, stringovi, brojevi, nizovi i objekti-->
<script>
export default {
data() {
  return {
    title:'VUE OBUKA',
    number: 0

  }
},

methods:{
  addNumber(){
    this.number = this.number + 1
  },
  removeNumber(){
    this.number = this.number - 1
  },
  // funkcija koja radi i sabiranje i oduzimanje
  changeNumber(operation){
if (operation=='plus') {
  this.number = this.number + 1
} else if (operation == 'minus'){
  this.number--
}
//za ispis rezultata u conzoli
console.log(this.number)

//mozemo sve sto smo gore definisali mozemo u funkcijama da koristimo
this.title = this.title + ' ' + this.number
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
