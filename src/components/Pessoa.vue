<template>
    <div>
        <input v-model="nome" placeholder="Digite seu nome">
        <h2>Esta é a descrição de: {{ nome }}</h2>
        <input type="text" v-model="email">
        <Lista v-bind:email='email' />
    </div>
    
</template>

<script>
    import Lista from './Lista.vue'

export default {
    name: 'Pessoa',
    data(){
        return {
            nome: '',
            email: ''
        }
    },
    components:{
        Lista
    }
}
</script>