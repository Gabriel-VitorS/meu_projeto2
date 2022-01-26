<template>
    <form action="" @submit="enviarForm($event)">
        <div>
            <label for="">Nome</label>
            <input type="text" name="" v-model="nome" id="">
        </div>
        <div>
            <label for="">Sobrenome</label>
            <input type="text" name="" v-model="sobrenome" id="">
        </div>
        <button>Enviar</button>
    </form>
</template>

<script>
export default {
    name: 'Form',
    methods:{
        enviarForm(e){
            e.preventDefault()
            const nome = this.nome
            const sobrenome = this.sobrenome
            console.log(e)
            alert(nome + ' ' + sobrenome)
        }
    },
    data(){
        return{
            nome: '',
            sobrenome: ''
        }
    }
}
</script>

<style scoped>
    *{
        color: black;
    }
</style>