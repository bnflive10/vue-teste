<template>
    <div>
        <p>{{compEmail}}</p>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Utiliso as seguintes tecnologias</p>
        <ul v-for="(technology, index) in backend_tecnologies" :key="index">
            <li>{{technology}}</li>
        </ul>
        <p>Utiliso as seguintes tecnologias Frontend</p>
        <ul v-for="technology in frontend_tecnologies" :key="technology.id">
            <li>{{technology.language}}</li>
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
        props:{
            compEmail: String
        },
        data(){
            return {
                mostrar_email: false,
                esta_trabalhando: true,
                meu_link: 'https://www.google.com',
                texto_botao: 'Mostrar',
                backend_tecnologies: ['Node.js','PHP','Phython'],
                frontend_tecnologies: [
                    {id: 1, language: 'javascript'},
                    {id: 2, language: 'HTML'},
                    {id: 3, language: 'CSS'}
                ]
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