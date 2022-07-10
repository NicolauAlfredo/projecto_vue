<template>
  <div>
      <h1>Olá Vue!</h1>
      <p>Meu nome é {{ nome }}, tenho {{ idade }} anos de idade e trabalho como {{ profissao }}.</p>
  </div>
</template>

<script>
  export default {
    name: 'Primeiro',
    data() {
      return {
        nome: "Nicolau",
        idade: 23,
        profissao: "Programador"
      }
    }
  }
</script>