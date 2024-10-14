<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else > estou em busca de novas oportunidades</p>
        <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>JavaScript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>
        <div>
            <button @click="showEmail" >{{ textoBotao }}</button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p>Para acessar meu portfólio <a v-bind:href="meu_link" target="_blank" >basta clicar aqui</a></p>
        <Picture />
    </div>
</template>
<script>
import Picture from './form/Picture.vue';

export default {
    name: 'info',
    components: {
        Picture
    },
    data() {
        return {
            esta_trabalhando: false,
            mostrar_email: false,
            email:'jhefinho@email.com',
            meu_link: 'https://google.com',
            textoBotao: 'Mostrar e-mail'
        }
    },
    methods: {
        showEmail() {
            this.mostrar_email = !this.mostrar_email
            if(!this.mostrar_email) {
                this.textoBotao = 'Mostrar e-mail'
            } else {
                this.textoBotao = 'Esconde e-mail'
            }
        }
    }
}
</script>
