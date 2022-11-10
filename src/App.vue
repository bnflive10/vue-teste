<template>
  <h1>Ola Mundo!</h1>
  <PrimeiroComponente/>
  <LifeCycle/>
  <pessoa/>
</template>

<script>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import LifeCycle from './components/LifeCycle.vue';
import Pessoa from './components/Pessoa.vue';

export default {
  name: 'App',
  components:{
    PrimeiroComponente,
    LifeCycle,
    Pessoa
  }
}
</script>