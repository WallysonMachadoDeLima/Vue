<template>
  <div>
    <h1>-> NOVO</h1>
    <h2>Olá Vue!</h2>
    <p>Meu nome é {{ name }}, e trabalho como {{ profissao }}</p>
  </div>
</template>


<script>
export default {
  name: "PrimeiroComponente",
  data() {
    return {
      name: "Wallyson",
      profissao: "Dev Junior",
    };
  },
};
</script>
