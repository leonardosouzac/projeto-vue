<template>
    <h1>Na verdade meu nome é {{ nome }}</h1>
</template>

<script> 
export default {
    name: "LifeCycle",
    data () {
        return {
            nome: "Tefé"
        }

    },
    created(){
        setTimeout(() =>{
            this.nome = "CWB"
        }, 1000);
        
    },
    mounted(){
        setTimeout(() =>{
           this.nome = "Praia"
        }, 2000);
    },
    methods:{
        lifeCycle(){
            let i = 0;
            i++;
            console.log("Executou" + i);
        }
    }
}
</script>