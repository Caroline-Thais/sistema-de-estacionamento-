<template>
<div id="nav">
    <router-link to="/" id="logo-url">
        <img :src="logo" id="logo" :alt="alt">
    </router-link>

    
    <router-link to="/">Home</router-link>  
    <router-link to="/cadastro">Cadastro</router-link>
  </div>
</template>

<script>

export default{
  name: "Navbar",
  props: ["logo", "alt"] //Logo do projeto e as imagens
}

</script>

<style scoped>
#nav{
  background-color:azure;
  padding: 15px 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}

#nav #logo-url{
  margin: auto;
  margin-left: 0;
}

#logo{
  height: 50px;
  width: 50px;
}

#nav a{
  color: gray;
  text-decoration: none;
  margin: 12px;
  transition: .5s;
  font-size: 20px;
}

#nav a:hover{
  color: greenyellow;
  border-bottom: 2px solid greenyellow;
}



</style>
