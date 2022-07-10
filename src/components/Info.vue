<template>
    <div>
        <p v-if ="esta_trabalhando"> Estou a trabalhar no momento.</p>
        <p v-else> Estou em busca de novas oportunidades!</p>
        <p>Utilizo as seguintes tecnologias para back-end: </p>
        <ul>
            <li v-for="(technology, index) in backend_technologies" v-bind:key="index"> {{ technology }} </li> 
        </ul>

        <p>Utilizo as seguintes tecnologias para front-end: </p>
        <ul> 
            <li v-for="(technology) in frontend_technologies" :key="technology.id"> {{ technology.language }} </li> 
        </ul> 

        <div>
            <button @click="showEmail">{{ textoBotao }}</button>
        </div>
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p class="portifolio">Para acessar o meu portifólio basta <a v-bind:href="portfolio" target="_blank">clicar aqui</a></p>
        <Picture />
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
                mostrar_email: false,
                portfolio: "https://www.google.com",
                textoBotao: "Mostrar e-mail",
                backend_technologies: ['Java', 'Python', 'JavaScript'],
                frontend_technologies: [
                    {id: 1, language: 'HTML'},
                    {id: 2, language: 'CSS'},
                    {id: 3, language: 'Vue'}
                ]
            }
        },
        methods: {
            showEmail() {
                this.mostrar_email = !this.mostrar_email
                if(!this.mostrar_email) {
                    this.textoBotao = "Mostrar e-mail"
                } else {
                    this.textoBotao = "Esconder e-mail"
                }
            }
        }
    }
</script>