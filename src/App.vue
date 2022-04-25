<template>
<div>
<Navbar :logo="logo_src" :alt="app_name"/>
  <router-view/>
<Footer/>
</div>

</template>

<script>
  import Navbar from './components/Navbar.vue'
  import Footer from './components/Footer.vue'

export default {
 
 components:{
   Navbar,
   Footer
 },
 data(){
   return {
     logo_src: "/img/carro-ecologico.png",
     app_name: "Cadastre o carro no estacionamento"
   }
 }
}
</script>

<style>
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
}

.main-container{
  margin: 40px;
  min-height: 250px;
}

h1{
  text-align: center;
  font-size: 42px;
  margin-bottom: 40px;
  color: gray;
}

</style>
