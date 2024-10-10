<template>
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
    export default {
        name: 'LyfeCycle',
        data() {
            return {
                nome: 'ainda não sei'
            }
        },
        created() {
            setTimeout (() => {
                
            })
            this.nome = 'Jeferson'
        },
        mounted() {
            this.nome = 'bora borilll '
        }
    }
</script>
