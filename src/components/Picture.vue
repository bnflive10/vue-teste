<template>
    <div class="col-md-12">
        <img :src="logo" alt="">    
    </div>
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