<template>
  <div>
    <h1>-> MEME</h1>
    <h2>Meu meme é {{ meme }}</h2>
  </div>
</template>

<script>
export default {
  nome: "LifeCycle",
  data() {
    return {
      meme: "As avores somos nozes",
    };
  },
  created() {
    setTimeout(() => {
      this.meme = "Quiero café";
    }, 1000);
  },
  mounted() {
    setTimeout(() => {
      this.meme = "Hora do show";
    }, 2000);
  },
};
</script>
