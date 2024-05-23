<template>
  <div>
    <form class="formulario">
      <label for="nome">Nome:</label>
      <br />
      <input type="text" id="nome" name="nome" v-model="nome" />
      <br />
      <label for="dataNascimento">Data Nascimento:</label>
      <br />
      <input
        type="text"
        id="dataNascimento"
        name="dataNascimento"
        v-model="dataNascimento"
      />
      <br />
    </form>
  </div>
  <button class="botao" v-on:click="calcularIdade">Calcular Idade</button>
  <p style="text-align: center">{{ nome }} tem: {{ idade }}</p>
</template>

<script setup>
import { ref } from 'vue';

const nome = ref('Elias Santos');
const dataNascimento = ref(0);
const idade = ref(0);

function calcularIdade() {
  debugger;
  console.log(idade.value);
  console.log(dataNascimento.value);
  idade.value = 2024 - dataNascimento.value;
  console.log(idade.value);
  console.log(dataNascimento.value);
}
</script>

<style scoped>
.formulario {
  margin: 0 auto;
  padding: 5px;
  width: 200px;
  background-color: darkcyan;
}

.botao {
  margin: 5px auto;
  padding: 5px;
  display: block;
  background: darkcyan;
  border-radius: 5px;
  border-style: none;
  cursor: pointer;
}

.botao:hover {
  background-color: rgb(93, 155, 155);
}
</style>
