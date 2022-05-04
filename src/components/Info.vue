<template>
  <div>
    <Picture />
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de novas oportunidades.</p>
    <p>Utilizo as seguintes tecnologias:</p>
    <ul>
      <li>Go</li>
      <li>Rust</li>
      <li>Vue.js</li>
    </ul>
    <div>
      <button @click="showEmail">{{ textoBotao }}</button>
    </div>
    <p v-show="mostrar_email">Mande uma mensagem para {{ email }}</p>
    <p class="teste">
      Para acessar meu portfólio
      <a v-bind:href="meu_link" target="_blank">basta clicar aqui </a>
    </p>
  </div>
</template>


<script>
import Picture from "./Picture.vue";
export default {
  components: { Picture },
  name: "info",
  components: {
    Picture,
  },
  data() {
    return {
      esta_trabalhando: false,
      mostrar_email: false,
      email: "praiajew@vkontakte.com",
      meu_link: "https://ifood.com.br",
      textoBotao: "Mostrar e-mail"
    };
  },
  methods: {
    showEmail() {
        this.mostrar_email = !this.mostrar_email
        if(!this.mostrar_email){
            this.textoBotao ="Mostrar e-mail"
        } else {
            this.textoBotao ="Esconder e-mail"
        }
    },
  },
};
</script>