<template>
<info :email="email"/>
<Forms />
</template>

<script>
    import Info from './Info.vue'
    import Forms from './Forms.vue'
    export default{
        name: "Pessoa",
        components:{
            Info,
            Forms
        },
        data(){
            return {
                nome: 'Leonardo',
                email: 'joao@email.com'
            }
        }
    }
</script>
