<template>
    <h1>Meu nome é {{nome}}</h1>
</template>

<script>
export default{
    name: 'LifeCycle',
    data(){
        return{
            nome:"Ainda nao sei"
        }
    },
    created(){
        setTimeout(() => {
            this.nome = "Joao"
        }, 1000)
        
        
    },
    mounted(){
        setTimeout(() => {
            this.nome = "Bernardino"
        }, 2000)
        this.executar()
    },
    methods:{
        executar(){
            console.log('executou aaaaa');
        }
    }
}

</script>