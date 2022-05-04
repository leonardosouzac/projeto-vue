<template>
<div>
    <h1>Olá forasteiro,</h1>
    <p>Meu nome é {{ nome }} e vendo {{ profissao }}.</p>
</div>
</template>

<script> 
    export default{
        name: "PrimeiroComponente",
        data(){
            return {
                nome: "Leonardo",
                profissao: "porcos selvagens"
            }
        }
    }
</script>