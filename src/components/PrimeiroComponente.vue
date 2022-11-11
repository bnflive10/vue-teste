<template>
  <div class="col-md-12">
    <h1>Ola VUE!</h1>
    <p>meu nome é {{ nome }} sou {{profissao}}</p>
  </div>
</template>

<script>
export default {
  name: "PrimeiroComponente",
  data() {
    return {
      nome: "bnflive10",
      profissao: "Programador"
    };
  },
};
</script>