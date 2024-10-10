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
                this.nome = 'Jeferson'
            }, 1000)
        },
        mounted() {
            setTimeout (() => {
                this.nome = 'Bora Bill'
            }, 2000);
        }
    }
</script>
