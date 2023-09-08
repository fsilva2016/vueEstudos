<template>
    <div>
        <menuHeader />
        <new-componentes/>
        <lifeCyde/>
        <pessoa/>
    </div>
</template>
<script>
import menuHeader from './components/Header.vue';
import newComponentes from './components/NewComponentes.vue';
import lifeCyde from './components/LifeCycle.vue';
import pessoa from './components/Pessoa.vue'
export default {
    
    name:'App',
    components:{
        menuHeader,
        newComponentes,
        lifeCyde,
        pessoa
    },
    data() {
        return{
            nome:'Felipe'
        }
    }
}
</script>