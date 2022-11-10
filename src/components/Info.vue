<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Utiliso as seguintes tecnologias</p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>Phyton</li>
        </ul>
        <p>Para acessar o nosso portifolio <a v-bind:href="meu_link">Aqui!</a></p>
    </div>
</template>

<script>
    export default {
        name: "info",
        data(){
            return {
                esta_trabalhando: true,
                meu_link: 'https://www.google.com'
            }
        }
    }
</script>