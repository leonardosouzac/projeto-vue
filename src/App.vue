<template>
  <div>
    <Header :esta_logado="true"/>
    <PrimeiroComponente />
    <life-cycle />
    <Pessoa />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";

export default {
  name: "app",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Header,
  },
};
</script>

<style>
body {
  background-color: #333;
  color: #fff;
  margin: auto;
  width: 50%;
  border: 2px solid #DDD;
  padding: 40px;
}

a {
  color: rgba(255, 83, 83, 0.918);
}

.teste {
  background-color: #000;
}
</style>