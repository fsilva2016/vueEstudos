<template >
    <div>   
        <img :src="avatar" :alt="descripion">
        <p>{{descripion}}</p>
    </div>
</template>
<script>
export default {
    name:'userImagens',
    data(){
        return{
            avatar:'/img/pessoa.png',
            descripion:'Minha Primeira Foto'
        }
    }
}
</script>
<style >
    img{
        width: 150px;
    }
</style>