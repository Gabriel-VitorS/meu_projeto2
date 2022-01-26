<template>
  <Botoes />
  <ListaVue />
  <FormVue />
</template>

<script>
import Botoes from "./components/Botoes.vue";
import FormVue from './components/Form.vue';
import ListaVue from './components/Lista.vue';

  export default {
    name: 'App',
    components:{
      Botoes,
      ListaVue,
      FormVue
    }
  }
  
</script>

<style>
body{
  background-color: #333;
}

p{
  color: white;
}
</style>
