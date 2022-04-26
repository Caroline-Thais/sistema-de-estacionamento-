<template>
    <div>
        <div id="carro-form">
            <div class="input-container">
                <label for="name">Nome do cliente:</label>
                <input type="text" id="nome" v-model="nome" placeholder="nome">
            </div>

            <div class="input-container">
                <label for="carro">Carro:</label>
                <input type="text" id="carro" v-model="carro" placeholder="carro">
            </div>

            <div class="input-container">
                <label for="placa">Placa:</label>
                <input type="text" id="placa" v-model="placa" placeholder="placa">
            </div>

            <div class="input-container">
                <label for="hora">Horário de entrada:</label>
                <input type="text" id="hora" v-model="hora" placeholder="hora entrada">
            </div>

           <div class="input-container">
                
                <input type="submit" class="submit-btn" value="Cadastrar">
            </div>
        </div>
    </div>
</template>

<script>
//import { defineComponent } from '@vue/composition-api'

export default {
  name: "Carroform"
}
</script>

<style scoped>
#carro-form{
    max-width: 300px;
    margin: 0 auto;
}


.input-container{
    display: flex;
    flex-direction: column;
    margin-bottom: 20px;
}

label{
    font-weight: bold;
    margin-bottom: 15px;
    padding: 5px 10px;
    border-left: 4px solid greenyellow;
}

input{
    padding: 5px 10px;
    width: 300px;
}

.submit-btn{
    background-color: aquamarine;
    color: gray;
    padding: 10px;
    cursor: pointer;
}
</style>
