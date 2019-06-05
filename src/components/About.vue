<template lang="pug">
    section.about
        h2.about__title Расскажите о себе словами

        p.about__description Напишите пару предложений, чем вас привлекла наша вакансия и чего вы ожидаете от работы в CSSSR. Кстати, будет здорово, если при нехватке места для текста строки будут добавляться автоматически.

        article.about__story(contenteditable="true") 
            p Опытный удалёнщик. Работаю так с 2009 года. С тех пор сменил сферу деятельности и специальность, но удалёнка как стиль жизни и способ рабты - останется навсегда. Потому что работа это не место, это дело.
              

</template>

<script>
export default {
    name: 'About'    
}
</script>

<style lang="stylus" scoped>
    .about
        width: 100%
        padding: 15px 0
        display: flex
        flex-wrap: wrap

    .about__title
        width: 100%
        text-align: left
        font-size: 1.5em
        font-weight: 700
        line-height: 50px
        color: #2f1b15   

    .about__description
        width: 100%
        font-size: 15px
        font-weight: 400
        line-height: 23px
        color: #3d3d3d
        padding-bottom: 25px 

    .about__story
        width: 100%
        font-family: "CourierNewPSMT"
        font-size: 24px
        font-weight: 400
        line-height: 60px
        color: #231f20
        background-image: url("../assets/images/Horisontal.png")
        background-position: 0 16px 

        p 
            text-indent: 40px

        .dirty
            text-decoration: line-through 

    @media screen and (max-width: 767px)
        .about__story
            font-size: 20px
            line-height: 24px
            background: none 
            text-align: justify

            p
                text-indent: 20px            

</style>

