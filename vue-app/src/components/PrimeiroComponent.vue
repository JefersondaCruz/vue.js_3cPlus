<template>
    <div>
        <Reutilizacao />
        <h1>Olá vue!</h1>,
        <Reutilizacao />
        <p> Meu Nome é {{ nome }} e trabalho como {{ profissao }}</p>
        <MultiplosEventos />
        <Reutilizacao />
        <Reutilizacao />
        <Reutilizacao />
        <Reutilizacao />
        <Reutilizacao />
    </div>
</template>

<script>
    import MultiplosEventos from './MultiplosEventos.vue';  
    
    import Reutilizacao from './Reutilizacao.vue';

    export default{
        name: "PrimeiroComponent",
        components: {
            MultiplosEventos,
            Reutilizacao
        },
        data() {
            return {
                nome: 'MClovinn',
                profissao: 'Programador'
            }
        },
        
    }
</script>
