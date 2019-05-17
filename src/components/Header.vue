<template lang="pug">
    header.header
        .header__top
            img(src="../assets/images/Logo.png" alt="Logo" class="logo")
            img(src="../assets/images/Slogan.png" alt="Slogan" class="slogan")

        img(src="../assets/images/Delo.png" alt="Title" class="title")

</template>

<script>

export default {
    name: 'Header'
}

</script>

<style scoped lang="stylus">
    .header 
        width: 100%
        display: flex
        flex-direction: column
        align-items: center
        padding: 0 0 30px 0;
            
    .header__top 
        width: 100%
        display: flex
        justify-content: space-between
    
    .logo 
        width: 154px
        height: 52px
    
    .slogan 
        height: 252%
        height: 106px
        transform: translate(30px, -30px)  
    
    .title 
        width: 221px

    @media screen and (max-width: 767px)
        .logo
            width: 77px
            height: 26px

        .slogan
            width: 126px
            height: 53px
            transform: translate(10px, -30px)          
    
        .title
            width: 110px     
</style>


