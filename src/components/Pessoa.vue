<template>
    <div class="col-12">
        pessoa: {{nome}}
        <info compEmail="props email bnflive10@gmail.com"/>
        <Formulario/>
    </div>
</template>

<script>
import Info from './Info.vue';
import Formulario from './Form.vue';

export default {
    name:"Pessoa",
    data(){
        return{
            nome: "Bernardino",
            
        }
    },
    components:{
                Info,
                Formulario
            }
}
</script>