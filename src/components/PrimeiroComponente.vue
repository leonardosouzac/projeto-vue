<template>
<div>
    <h1>Olá forasteiro,</h1>
    <p>Meu nome é {{ nome }} e vendo {{ profissao }}.</p>
    <MultiplosEventos />
</div>
</template>

<script> 
    import MultiplosEventos from './MultiplosEventos.vue'

    export default{
        name: "PrimeiroComponente",
        components: {
            MultiplosEventos
        },
        data(){
            return {
                nome: "Leonardo",
                profissao: "porcos selvagens"
            }
        }
    }
</script>