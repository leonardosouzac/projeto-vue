<template>
    <h1>Meu nome é {{ nome }}</h1>
</template>

<script> 
export default {
    name: "LifeCycle",
    data () {
        return {
            nome: "dunno yet"
        }
    },
    created(){
        setTimeout(() =>{
            this.nome = "CWB"
        }, 1000)
    },
    mounted(){
        setTimeout(() =>{
           this.nome = "Praia"
        }, 2000)
    }
}
</script>