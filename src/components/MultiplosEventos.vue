<template>
    <div>
        <button @click="acionarEventos">Ativar Múltiplos eventos </button>
        <p>{{variosEventos}}</p>
    </div>
</template>
<script>
export default {
    name:'MultiplosEventos',
    data(){
        return{
            variosEventos:''
        }
    },methods: {
        acionarEventos(){
            this.variosEventos = 'oiiii'
        }
    },
}
</script>