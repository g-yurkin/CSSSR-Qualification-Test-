<template lang="pug">
    main.info
        div.info__line
            span.info__query Полное ФИО
            span.info__answer Ященко Юрий Алексеевич    
        
        div.info__line
            span.info__query Год рождения
            span.info__answer 1976    
        
        div.info__line
            span.info__query Место жительства
            span.info__answer г. Рубцовск    
        
        div.info__line
            span.info__query Скайп
            span.info__answer g.yurkin    
        
        div.info__line
            span.info__query Почта
            span.info__answer yurkin@mail.ru    
</template>

<script>
export default {
    name: 'Info'
}
</script>

<style scoped lang="stylus">
    .info 
        width: 100%
        display: flex
        flex-direction: column
        align-items: stretch
        padding: 30px 0 5px 0
    
    .info__line
        width: 100%
        height: 63px  
        display: flex
        flex-wrap: wrap
            
    .info__query 
        font-family: 'PT Sans', sans-serif
        font-size: 1.375em
        font-weight: 700
        line-height: 60px
        color: #2f1b15
        flex-basis: content
        padding: 0 1em 0 0

    .info__answer
        font-family: 'CourierNewPSMT'
        font-size 1.875em
        font-weight 400
        line-height: 40px
        color: #231f20
        flex-basis: content
        flex-grow: 1
        height: 60px
        padding: 0 10px
        background-image url("../assets/images/Horisontal.png")
        background-position: 0 72px 

    @media screen and (max-width: 767px)
        .info__line
            height: 120px 
            flex-wrap: nowrap
            flex-direction: column

        .info__answer
            font-size: 1.2em
            padding: 0     
 
</style>