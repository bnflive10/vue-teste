<template>
    <div>
        pessoa: {{nome}}
        <info/>
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