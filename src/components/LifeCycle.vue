<template>
    <h1>Meu nome é:{{nome}}</h1>
</template>
<script>
    export default {
        name:'liveCycle',
        data(){
            return{
                nome:'Ainda não sei',
            }
        },
        created() {
            setTimeout(() =>{
                this.nome
            },2000)
            this.lifeCycle()
        },
        mounted() {
            this.nome ='Pedro'
        },
        methods: {
            lifeCycle(){
                console.log('Ola')
            }
        },
    };
</script>
<style scoped>
    h1{
        color: red;
    }
</style>