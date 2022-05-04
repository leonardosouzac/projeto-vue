<template>
    <img :src="avatar" :alt="descricao">
</template>

<script>
export default{
    name: 'Picture',
    data(){
        return {
            avatar: "/img/avatar.jpg",
            descricao: "Eren Yeager"
        }
    }
}
</script>