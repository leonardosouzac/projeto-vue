<template>
  <h2>Meu formulário:</h2>
  <form action="" @submit="enviarFormulario($event)">
    <input type="text" v-model="name" placeholder="nome" /><br />
    <input type="text" v-model="email" placeholder="email" /><br />
    <input type="submit" value="Enviar" />
  </form>
  <p>Conteúdo</p>
  <p>Conteúdo</p>
  <p>Conteúdo</p>
</template>

<script>
export default {
  name: "Forms",
  data() {
    return {
      name: "",
      email: "",
    };
  },
  methods: {
    enviarFormulario(e) {
      e.preventDefault();

      const name = this.name;
      const email = this.email;

      console.log("form enviado pai");
      console.log ("O nome é " + name);
      console.log ("O email é " + email);

      //ajax p/ servidor para inserir o usuário
    },
  },
};
</script>

<style scoped>
p {
  margin: 150px;
}
</style>