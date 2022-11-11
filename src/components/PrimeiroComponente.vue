<template>
  <div class="col-md-12">
    <h1>Ola VUE!</h1>
    <p>meu nome é {{ nome }} sou {{profissao}}</p>
    <MultiplosEventos/>
  </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue';

export default {
  name: "PrimeiroComponente",
  data() {
    return {
      nome: "bnflive10",
      profissao: "Programador"
    };
  },
  components:{
    MultiplosEventos
  }
};
</script>