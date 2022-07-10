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
    </div>
</template>

<script>
    export default {
        name: 'Info',
        data() {
            return {
                email: "nicolaualfredo@yahoo.com",
                esta_trabalhando: false,
                mostrar_email: true
            }
        }
    }
</script>