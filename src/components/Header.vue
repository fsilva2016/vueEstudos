<template>
    <div>
        <ul>
            <li v-for="item in menu" :key="item.id"> {{item.name}}</li>
        </ul>
    </div>
</template>
<script>
    export default {
        name:'AppHeader',
        data(){
            return{
                menu:[
                    {id:1,name:'Home'},
                    {id:2,name:'Menu'},
                    {id:3,name:'Contatos'}
                ]
            }
        }
    }
</script>
<style>
    ul{
        display: flex;
        list-style: none;
        background: white;
        column-gap: 10px;
        cursor: pointer;
    }
    a{
        color: blue;
        text-decoration: none;
        transition: .5s;
    }
    a:hover{
        color: pink;
    }
</style>