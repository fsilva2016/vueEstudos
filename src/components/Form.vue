<template>
   <form action="" @submit="enviarFormulario($event)">
        <!-- <div>
            <inputText />
        </div>    -->
        <div>
            <input type="text" name="" id="" v-model="name">
        </div>    
           <div>
            <input type="text" name="" id="" v-model="email">
        </div>   
        <div>
            <inputSubmit/>
        </div>
   </form>
</template>
<script>
    // import inputText from './Form/InputText.vue';
    import inputSubmit from './Form/InputSubmit.vue';
    export default {
        name:'formInput',
        components:{
            // inputText,
            inputSubmit,
        },
        data(){
           return{
                name:"",
                email:""
           }
            
        },
        methods:{
            enviarFormulario(e){
                e.preventDefault();

                const email = this.email;
                const name = this.name;
                
                console.log('Formulario Enviado com sucesso')
                console.log(name, email)
            
            }

        }
        
    }
</script>
<style scoped>
    div{
        margin-bottom: 10px;
    }
</style>