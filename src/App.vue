<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <h1>Method Properties</h1>
  <h3>My handle is {{ name }}</h3>
  <h3>The first number: {{ firstNumber }}</h3>
  <h3>The second number: {{ secondNumber }}</h3>
  <h3>Result: {{  multiply(firstNumber,secondNumber) }}</h3>
  <section style="align:left">
  <label for="firstN">First Number: </label>
  <input id="firstN" type="number" placeholder="Enter first number" v-model="firstNumber">

  <label for="secondN">Second Number: </label>
  <input id="secondN" type="number" placeholder="Enter second number" v-model="secondNumber">


  </section>
  <footer>Year {{ year() }}</footer>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data(){
    return {
      name:"dnlsyfq",
      prefix:20,
      suffix:24,
      firstNumber:'',
      secondNumber:''
    }
  },
  components: {
    // HelloWorld
  },
  methods: {
    fullName(){
      return 'dnlsyfq' ;
    },
    year(){
      return this.prefix + '' + this.suffix;
    },
    multiply(firstNumber,secondNumber){
      return firstNumber * secondNumber
    }
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
  margin-top: 60px;
}
</style>
