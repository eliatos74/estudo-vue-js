<template>
  <NavBar />
  <header>
    <Cabecalho />
  </header>
  <main>
    <Usuario />
  </main>
</template>

<script setup>
import Cabecalho from './components/Cabecalho.vue';
import NavBar from './components/NavBar.vue';
import Usuario from './components/Usuario.vue';
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}

header {
  line-height: 1.5;
}
</style>
