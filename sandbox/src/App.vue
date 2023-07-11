<template>
  <Header :esta_logado=true />
  <LifeCycle/>
  <Pessoa/>
  <Formulario/>
  <MultiplosEventos/>
  <Reutilizacao/>
  <Reutilizacao/>
</template>

<script>
import LifeCycle from './components/form/LifeCycle.vue';
import Pessoa from './components/form/Pessoa.vue';
import Header from './components/form/Header.vue'
import Formulario from './components/form/Formulario.vue';
import MultiplosEventos from './components/form/MultiplosEventos.vue';
import Reutilizacao from './components/form/Reutilizacao.vue';

export default {
  name: 'App',
  components: {
    LifeCycle,
    Pessoa,
    Header, 
    Formulario,
    MultiplosEventos,
    Reutilizacao
  }
}
</script>

<style>

#app {
  font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
}
body {
  background-color: cornflowerblue;
  color: black;
}
a {
  text-decoration: none;
  color: darkorange;
}

</style>