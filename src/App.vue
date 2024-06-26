<template>
  <PrimeiroComponente />
  <LifeCycle />
  <PessoaId />
</template>

<script>
  import PrimeiroComponente from './components/PrimeiroComponente.vue';
  import LifeCycle from "./components/LifeCycle.vue";
  import PessoaId from "./components/PessoaId.vue";
  
  export default {
    name: "App",
    components: {
      PrimeiroComponente,
      LifeCycle,
      PessoaId
    }
  }
</script>