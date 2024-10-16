<template>
    <div>
        <img :src="stranger" :alt="descricao">
        <MudarImagem @mudar-Imagem="trocarImagem"/>
    </div>
</template>
<script>
import MudarImagem from '../MudarImagem.vue';
export default {
    name:'Picture',
    components: { 
        MudarImagem
    },
    data() {
        return{
            stranger: "/img/ponei.png",
            descricao: "Jeferson img"
        }
    },
    methods: {
        trocarImagem() {
            this.stranger = "/img/car.png"
        }
    }
}
</script>

