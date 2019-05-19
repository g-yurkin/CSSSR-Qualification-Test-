<template lang="pug">
    section.checkboxes
        h2.checkboxes__title Расскажите о себе чекбоксами

        p.checkboxes__description Отметьте чекбоксами пункты, которые соответствуют вашим скиллам. Кстати, отсутствие опыта не означает, что у вас меньше шансов стать одним из наших товарищей. Это означает, что вы будете получать те задачи, с которыми гарантировано будете справляться.

        .checkboxes__container
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | БЭМ/OOCSS
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Pug (Jade)
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Stylus/LESS/SASS
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Работаю с SVG
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Верстаю семантично
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox")
                span.checkboxes__picture
                | Acessibility (A11Y)
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox")
                span.checkboxes__picture
                | ES2015/2016

        .checkboxes__container
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Gulp/GRUNT
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox")
                span.checkboxes__picture
                | Webpack
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox")
                span.checkboxes__picture
                | Дружу с WebGL
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | jQuery
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox")
                span.checkboxes__picture
                | Знаю/изучаю Angular
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Знаю/изучаю React
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Знаю/изучаю Node.js

        .checkboxes__container
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Использую Git
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | С глазомером всё ок
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Читаю <a href="http://blog.csssr.ru">blog.csssr.ru</a>
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | Я ленивый
            label.checkboxes__check
                input(class="checkboxes__input" type="checkbox" class="checkbox" checked)
                span.checkboxes__picture
                | У меня хороший английский
                                    
</template>

<script>
export default {
    name: 'Checkboxes'
}
</script>

<style lang="stylus" scoped>
    .checkboxes
        width: 100%
        padding: 30px 0 15px 0
        display: flex
        flex-wrap: wrap

    .checkboxes__title
        width: 100%
        text-align: left
        font-size: 1.5em
        font-weight: 700
        line-height: 50px
        color: #2f1b15   

    .checkboxes__description
        width: 100%
        font-size: 15px
        font-weight: 400
        line-height: 23px
        color: #3d3d3d
        padding-bottom: 16px  

    .checkboxes__container
        width: calc(100% / 3)
        display: flex
        flex-direction: column
           
    
    .checkboxes__check
        padding: 5px 0 5px 1.2em 
        font-size: 1.375em
        font-weight: 700
        line-height: 25px
        color: #000
    
    .checkboxes__input
        position: absolute
        appearance: none

    .checkboxes__picture
        position: absolute
        margin-left: - 1.2em
        margin-top: 4px
        width: 19px
        height: 18px
        background-image url("../assets/images/Shape_2.png")
        background-size: contain 

    .checkboxes__input:checked + .checkboxes__picture::after
        content: ""
        display: block
        width: 19px
        height: 30px
        margin: -10px 0 0 3px 
        background-image url("../assets/images/Marker.png")
        z-index: 9

    @media screen and (max-width: 960px) 
        .checkboxes
            flex-direction: column

        .checkboxes__container
            width 100%    
    
    

</style>
