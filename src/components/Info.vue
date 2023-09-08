<template>
    <div>
        <imagens/>
        <p v-if="estaEstudando"> Estou estudando</p>
        <p v-else> não estou estudando</p>
        <p>Estou estudando as novas tecnologias </p>
        <ul>
            <li v-for="(front, index) in frontEndTecnoligia" :key="index"> 
                {{front}}
            </li>
        </ul>
        <p>
            Lista que ainda tem que estudar 
        </p>
        <ul>
            <li v-for="list in futurosEstudos" :key="list.id" >
                {{list.languege}}
            </li>
        </ul>
        <div>
            <button @click="showEmail">
                <p>{{textButton}}</p>
            </button>
        </div>
        <p v-show="mostraEmail">Mande mensagem para : {{email}}</p>
        <p>Para ver meu portfólio <a v-bind:href="meuLink" target="_black">Acessar</a> </p>
    </div>
</template>
<script>
import imagens from './Picture.vue'
export default {
    name:'infoPessoal',
    components:{
        imagens
    },
    data() { 
        return{
            name:'PHP',
            estaEstudando:true,
            mostraEmail:false,
            email:'felipedasilva1990@yahoo.com.br',
            meuLink:'https://www.google.com.br',
            textButton:'Mostra meu Email',
            frontEndTecnoligia:['html','css','JS','jquery','react','vue'],
            futurosEstudos:[
                {id:1, languege:'React'},
                {id:2, languege:'Angular'},
                {id:3, languege:'Java'},
                {id:4, languege:'React'},
                {id:5, languege:'React'}
                ]
        }
    },
    methods: {
        showEmail(){
            this.mostraEmail = !this.mostraEmail
            if(!this.mostraEmail){
                this.textButton = 'Mostra meu Email'
            }else{
                this.textButton = 'Oculta email'
            }
        }
    },
}
</script>