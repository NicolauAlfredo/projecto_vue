<template>
    <First/>
</template>

<script>
    import First from './components/First.vue'
    import LifeCycle from './components/LifeCycle.vue' 

    export default {
        name: "App",
        components: {
            First,
            LifeCycle
        }
    }
</script>