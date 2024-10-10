<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else ></p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>JavaScript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>
    </div>
</template>
<script>
export default {
    name: 'info',
    data() {
        return {
            esta_trabalhando: true
        }
    }
}
</script>
