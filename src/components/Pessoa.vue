<template>
    <div>
        <h2>Essa e a descrição da pessoa {{name}}</h2>   
        <Form/> 
        <infoPessoal/>
    </div>

</template>
<script>
import Form from'./Form.vue'
import infoPessoal from './Info.vue'
export default {
    name:'dadosPessoa',
    components:{
        Form,
        infoPessoal
    },
    data(){
        return{
            name:'Felipe'
        }
    }
}
</script>