<template>
  <div>
    <PrimeiroComponente />
    <p>na data {{ date }}</p>
    <LifeCycle />
    <Pessoa />
  </div>
</template>


<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";
export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
  },
  data() {
    return {
      date: "14/11/2022",
    };
  },
};
</script>