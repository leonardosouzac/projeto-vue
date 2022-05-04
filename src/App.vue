<template>
<div>
  <Header />
  <PrimeiroComponente />
  <life-cycle />
  <Pessoa />
</div>
</template>

<script>
  import Header from './components/Header.vue'
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import Pessoa from './components/Pessoa.vue'

  export default{
    name: "app",
    components: {
      PrimeiroComponente,
      LifeCycle,
      Pessoa,
      Header,
    }
  }
</script>

<style>
  body{
    background-color: #333;
    color: #FFF;
  }

  a {
    color: rgba(255, 83, 83, 0.918);
  }

  .teste{
    background-color: #000;
  }
</style>