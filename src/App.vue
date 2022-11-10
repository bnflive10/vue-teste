<template>
  <div class="container-fluid">
    <div class="row">

      <div class="col-2">
        <Picture/>
      </div>
    </div>
    <h1>Ola Mundo!</h1>
    <PrimeiroComponente />
    <LifeCycle />
    <pessoa />
  </div>
</template>

<script>
import PrimeiroComponente from "./components/PrimeiroComponente.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";
import Picture from "./components/Picture.vue";

export default {
  name: "App",
  components: {
    PrimeiroComponente,
    LifeCycle,
    Pessoa,
    Picture,
  },
};
</script>