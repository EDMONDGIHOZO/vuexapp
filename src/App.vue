<template>
  <div id="app">
    <first-list v-bind:products="products"></first-list>
    
    <second-list v-bind:products="products"></second-list>
  </div>
</template>

<script>
import Firstlist from './components/productListOne.vue';
import SecondList from './components/productListTwo.vue';


export default {
  name: 'App',
  components: {
    'first-list': Firstlist,
    'second-list': SecondList
  },
  data(){
    return {
      products: [
        {name: 'Banana' , price: 2000}, 
        {name: 'Rice' , price: 230}, 
        {name: 'anana' , price: 400}, 
        {name: 'cabbage' , price: 24300}, 
        {name: 'milk' , price: 23000}, 
        {name: 'matoke' , price: 2450}, 
        {name: 'beans' , price: 2000}, 
        {name: 'cassava' , price: 1000}, 
        {name: 'maize' , price: 54000}, 

      ]
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
  width: 80%;
  margin: 0 auto;
}
</style>
