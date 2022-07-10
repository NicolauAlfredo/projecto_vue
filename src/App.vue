<template>
    <div>
        <Cabecalho/>
        <Primeiro/>
        <LifeCycle/>
        <Pessoa/>
    </div>    
</template>

<script>  

    import Cabecalho from './components/Cabecalho.vue'
    import Primeiro from './components/Primeiro.vue'
    import LifeCycle from './components/LifeCycle.vue' 
    import Pessoa from './components/Pessoa.vue'

    export default {
        name: "App",
        components: {
            Cabecalho,
            Primeiro,
            LifeCycle,
            Pessoa
        }
    }
</script>


<style>
    body {
        background-color: #333;
        color: white;
    }

    a {
        color: red;
    }

    .portifolio {
        background-color: blue;
    }
</style>