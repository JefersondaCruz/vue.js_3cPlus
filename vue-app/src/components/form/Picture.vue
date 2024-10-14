<template>
    <img :src="stranger" :alt="descricao">
</template>
<script>
export default {
    name:'Picture',
    data() {
        return{
            stranger: "/img/stranger.jpg",
            descricao: "Jeferson img"
        }
    }
}
</script>

