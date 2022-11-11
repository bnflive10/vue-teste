<template>
  <button @click="primeiro($event), segundo($event)" class="btn btn-primary">
    Ativar Multiplos eventos
  </button>
  <p>{{ multiplos_eventos }}</p>
</template>

<script>
export default {
  name: "MultiplosEventos",
  data() {
    return {
      multiplos_eventos: "",
    };
  },
  methods: {
    primeiro(e) {
      this.multiplos_eventos = "Primeiro evento activado";
    },
    segundo(e) {
      setTimeout(() => {
        this.multiplos_eventos = "Segundo evento activado";
      }, 1000);
    },
  },
};
</script>