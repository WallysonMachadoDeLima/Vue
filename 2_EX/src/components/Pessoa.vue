<template>
  <div>
    <h1>-> PESSOA</h1>
    <h2>Está é a descrição da pessoa: {{ name }}</h2>
    <p>{{ name }} está utilizando as seguintes linguagens:</p>
    <Info />
    <Form />
  </div>
</template>

<script>
import Info from "./Info.vue";
import Form from "./Form.vue";

export default {
  nome: "Pessoa",
  components: {
    Info,
    Form,
  },
  data() {
    return {
      name: "Neymar Inassio",
    };
  },
};
</script>
