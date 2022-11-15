<template>
  <div>
    <ul>
      <li>JavaScript</li>
      <li>HTML</li>
      <li>CSS</li>
    </ul>
    <div id="trabalho">
      <!-- <p >{{ status_label }}</p> -->
      <p v-if="status_trabalho">Estou trabalhando</p>
      <p v-else>Não Estou trabalhando</p>
      <button v-on:click="trocar">{{ status_trabalho }}</button>
      <p v-show="mostrar_gmail">Mande uma mensagem para: {{ gmail }}</p>
      <p>
        Para acessar meu portifólio
        <a v-bind:href="portifolio">Basta Clicar aqui </a>
      </p>
      <Picture />
    </div>
  </div>
</template>
    
<script>
import Picture from "./Picture.vue";

export default {
  nome: "Info",
  components: {
    Picture,
  },
  data() {
    return {
      name: "Neymar Inassio",
      status_trabalho: true,
      status_label: "Estou trabalhando",
      mostrar_gmail: true,
      gmail: "machadodelimawallyson@gmail.com",
      portifolio: "https://www.linkedin.com/in/wallyson-machado/",
    };
  },
  methods: {
    trocar: function (e) {
      this.status_trabalho = !this.status_trabalho;

      //   this.status_label = this.status_trabalho
      //     ? "Estou trabalhando"
      //     : "Não estou trabalhando";
    },
  },
};
</script>
    