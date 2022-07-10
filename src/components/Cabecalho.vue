<template>
    <div>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">Projectos</a></li>
            <li><a href="#">Contactos</a></li>
        </ul>
    </div>
</template>

<script>

    export default {
        name: 'Cabecalho'
    }
</script>

<style scoped>
    ul {
        list-style: none;
        display: flex;    
        background-color: #999;    
    }

    li {
        margin-right: 10px;
    }

    a {
        color: #ddd;
        text-decoration: none;
        transition: .5s;
    }

    a:hover {
        color: turquoise;
    }
</style>