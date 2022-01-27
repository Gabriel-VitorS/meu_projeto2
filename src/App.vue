<template>
  <div>
  <Botoes />
  
  <FormVue />
  <Pessoa />
  </div>
  
</template>

<script>
import Botoes from "./components/Botoes.vue";
import FormVue from './components/Form.vue';
import ListaVue from './components/Lista.vue';
import Pessoa from './components/Pessoa.vue'

  export default {
    name: 'App',
    components:{
      Botoes,
      ListaVue,
      FormVue,
      Pessoa,
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
