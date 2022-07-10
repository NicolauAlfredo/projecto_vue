<template>
    <div>
        <Primeiro/>
        <LifeCycle/>
        <Pessoa/>
    </div>    
</template>

<script>  

    import Primeiro from './components/Primeiro.vue'
    import LifeCycle from './components/LifeCycle.vue' 
    import Pessoa from './components/Pessoa.vue'

    export default {
        name: "App",
        components: {
            Primeiro,
            LifeCycle,
            Pessoa
        }
    }
</script>