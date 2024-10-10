<template>
    <div>
        <h1>Olá vue!</h1>
        <p> APOIO O COMUNISMO {{ nome }} e trabalho como {{ profissao }}</p>
    </div>
</template>

<script>
    export default{
        name: "PrimeiroComponent",
        data() {
            return {
                nome: 'MClovinn',
                profissao: 'Programador'
            }
        },
        
    }
</script>
