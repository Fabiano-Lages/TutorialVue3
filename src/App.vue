<template>
  <HeaderPage />
  <PrimeiroComponente />
  <LifeCycle />
  <PessoaId />
</template>

<script>
  import HeaderPage from './components/HeaderPage.vue';
  import PrimeiroComponente from './components/PrimeiroComponente.vue';
  import LifeCycle from "./components/LifeCycle.vue";
  import PessoaId from "./components/PessoaId.vue";
  
  export default {
    name: "App",
    components: {
      HeaderPage,
      PrimeiroComponente,
      LifeCycle,
      PessoaId
    }
  }
</script>
<style>
  body {
    background-color: #333;
    color: #fff;
  }

  a {
    color: red;
  }
</style>