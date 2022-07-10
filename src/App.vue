<template>
    <Primeiro/>
    <LifeCycle/>
</template>

<script>  
       
    //import first from './components/first.vue'
    import LifeCycle from './components/LifeCycle.vue' 
    import Primeiro from './components/Primeiro.vue'

    export default {
        name: "App",
        components: {
            Primeiro,
            LifeCycle
        }
    }
</script>