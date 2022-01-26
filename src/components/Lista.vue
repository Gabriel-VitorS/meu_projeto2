<template>
    <p>Usa as seguintes tecnologias para backend: </p>
    <ul>
        <li v-for="(linguagens, index) in backend" v-bind:key="index">{{linguagens}}</li>
    </ul>

    <p>Usa as seguintes tecnologias para front: </p>
    <ul>
        <li v-for="linguagens in front" v-bind:key="linguagens.id"> {{linguagens.linguagem}}</li>
    </ul>
</template>

<script>
export default {
    name:'Lista',
    data(){
        return{
            backend: ['Node', 'PHP', 'C#', 'Java', 'Python'],
            front: [
                {id: 1, linguagem: 'Vue'},
                {id: 2, linguagem: 'HTML'},
                {id: 3, linguagem: 'CSS'},
                {id: 4, linguagem: 'JS'},
            ]
        }
    }
}
</script>

<style scoped>
    *{
        color: white;
    }
</style>