<template>
  <form action=""  method="post">
    <InputTextVue/>
    <SubmitVue/>
  </form>
</template>

<script>
import InputTextVue from './form_inputs/InputText.vue';
import SubmitVue from './form_inputs/Submit.vue';

 export default {
    name: "Formulario",
    components:{
        InputTextVue,
        SubmitVue
    }
 }

</script>