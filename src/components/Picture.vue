<template>
    <img :src="logo" alt="">
</template>

<script>
    export default {
        name: "Picture",
        data(){
            return{
                logo: '/img/logo-nagex.png'
            }
        }
    }
</script>