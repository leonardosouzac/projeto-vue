<template>
<div>
    <h1>Olá forasteiro,</h1>
    <Reutilizacao />
    <p>Meu nome é {{ nome }} e vendo {{ profissao }}.</p>
    <MultiplosEventos />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
    <Reutilizacao />
</div>
</template>

<script> 
    import Reutilizacao from './Reutilizacao.vue'
    import MultiplosEventos from './MultiplosEventos.vue'

    export default{
        name: "PrimeiroComponente",
        components: {
            MultiplosEventos,
            Reutilizacao
        },
        data(){
            return {
                nome: "Leonardo",
                profissao: "porcos selvagens"
            }
        }
    }
</script>