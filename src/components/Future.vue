<template lang="pug">
    section.future
        h2.future__title Какие у вас планы на будущее?

        p.future__description Этот ответ ни на что не повлияет. Не беда, если в будущем ваши планы поменяются.

        form.future__plan
            label.variant
                input(type="radio" name="choice" class="variant__input")
                span.variant__marker
                | Верстать

            label.variant
                input(type="radio" name="choice" class="variant__input" checked)
                span.variant__marker
                | Прокачиваться в JS

            label.variant
                input(type="radio" name="choice" class="variant__input")
                span.variant__marker
                | Менеджерство

            label.variant
                input(type="radio" name="choice" class="variant__input")
                span.variant__marker 
                | Другое            
</template>

<script>
export default {
    name: 'Future'
}
</script>

<style lang="stylus" scoped>
    .future
        width: 100%
        padding: 30px 0
        display: flex
        flex-wrap: wrap

    .future__title
        width: 100%
        text-align: left
        font-size: 1.5em
        font-weight: 700
        line-height: 50px
        color: #2f1b15   

    .future__description
        width: 100%
        font-size: 15px
        font-weight: 400
        line-height: 23px
        color: #3d3d3d
        padding-bottom: 16px 

    .future__plan
        font-size: 20px
        font-weight: 700
        line-height: 25px
        color: #000
        padding-top: 4px 

    .variant
        padding: 0 25px 0 30px
        position: relative

    .variant__input
        appearance: none

    .variant__marker
        position: absolute
        left: -10px
        top: -10px
        // margin-left: -30px
        display: block
        width: 41px
        height: 45px 
        background-image: url("../assets/images/Ellips-1.png") 

    .variant__input:checked + .variant__marker::after
        content: ''
        display: block
        width: 23px
        height: 27px
        position: absolute 
        top: 13px
        left: 9px
        background-image: url("../assets/images/Ellips-2.png")

    @media screen and (max-width: 767px)
        .future__plan
            width: 100%
            display: flex
            flex-direction: column  

        .variant                     
           margin-bottom: 20px
</style>

