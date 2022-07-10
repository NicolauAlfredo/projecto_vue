<template>
    <div>
        <p v-if ="esta_trabalhando"> Estou a trabalhar no momento.</p>
        <p v-else> Estou em busca de novas oportunidades!</p>
       <p>Utilizo as seguintes tecnologias: </p>
        <ul>
            <li>Java</li>
            <li>Python</li>
            <li>JavaScript</li>
            <li>PHP</li>
        </ul>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p>Para acessar o meu portifólio basta <a v-bind:href="portfolio" target="_blank">clicar aqui</a></p>
        <Picture/>
    </div>
</template>

<script>
    import Picture from './Picture.vue'

    export default {
        name: 'Info',
        components: {
            Picture
        },
        data() {
            return {
                email: "nicolaualfredo@yahoo.com",
                esta_trabalhando: false,
                mostrar_email: true,
                portfolio: "https://www.google.com"
            }
        }
    }
</script>