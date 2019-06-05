<template lang="pug">
    footer.data
        span.data__query Дата заполнения

        span.data__answer 18.05.2019

</template>

<script>
export default {
    name: 'Footer'
}
</script>

<style lang="stylus" scoped>
    .data
        width: 100%
        padding-top: 50px
        display: flex
        
    .data__query
        font-size: 22px
        font-weight: 700
        line-height: 50px
        color: #2f1b15
        padding-right: 16px

    .data__answer
        font-family: 'CourierNewPSMT'
        font-size: 30px
        line-height: 36px
        padding: 0 16px
        background-image: url('../assets/images/Horisontal.png')
        background-position 0 6px


    @media screen and (max-width: 767px)
        .data
            flex-direction: column     

</style>

