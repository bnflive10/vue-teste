<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Utiliso as seguintes tecnologias</p>
        <ul v-for="technology in backend_tecnologies">
            <li>{{technology}}</li>
        </ul>
        <div>
            <button class="btn btn-primary btn-sm" @click="showEmail">{{texto_botao}}</button>
        </div>
        <p v-show="mostrar_email">bnflive10@gmail.com</p>
        <p>Para acessar o nosso portifolio <a v-bind:href="meu_link">Aqui!</a></p>
    </div>
</template>

<script>
    export default {
        name: "info",
        data(){
            return {
                mostrar_email: false,
                esta_trabalhando: true,
                meu_link: 'https://www.google.com',
                texto_botao: 'Mostrar',
                backend_tecnologies: ['Node.js','PHP','Phython']
            }
        },
        methods:{
            showEmail(){
                
                this.mostrar_email = !this.mostrar_email
                if(this.mostrar_email == false){
                    this.texto_botao = 'Mostrar'
                }else{
                    this.texto_botao = 'Esconder'
                }
            }
        }
    }
</script>