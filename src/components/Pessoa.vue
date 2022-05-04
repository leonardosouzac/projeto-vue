<template>
<info />
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
        }
    }
</script>
