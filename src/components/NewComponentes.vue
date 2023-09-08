<template>
    <div>
        <h1>Ola Mundo</h1>
        <p>Menu Nome é: {{nome}}, eu trabalho como {{profision}}</p>
        <MultiplosEventos />
    </div>
</template>
<script>
import MultiplosEventos from './MultiplosEventos.vue';
export default {
    name:'newComponente',
    components:{
        MultiplosEventos
    },
    data(){
        return{
            nome:'Felipe Moraes',
            profision:'Front end pleno'
        }
    }
}
</script>