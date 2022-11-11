<template>
    <Header />
  <Picture />

  <div>
    <h1>Ola Mundo!</h1>
  </div>

  <PrimeiroComponente />
  <LifeCycle />
  <pessoa />
</template>

<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";
import Picture from "./components/Picture.vue";
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Picture,
    Header,
  },
};
</script>