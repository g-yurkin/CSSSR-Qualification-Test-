<template lang="pug">
    section.leveljs
        h2.leveljs__title Уровень владения JavaScript

        div.leveljs__indicator
            div(class="progress" id="progress")   
                div(class="marker" id="marker" v-bind:style="{left: level}")
            div(class="first-part" v-on:click="levelLow") Не владею
            div(class="second-part" v-on:click="levelMiddle") Использую готовые решения
            div(class="third-part" v-on:click="levelHiMiddle") Использую готовые решения и умею их переделывать
            div(class="fourth-part" v-on:click="levelHi") Пишу сложный JS с нуля

</template>

<script>
    export default {
        
        name: 'LevelJS',

        data: function() {
            return {
                level: '89%'
            }    
        },
        methods: {
            levelLow: function() {
                this.level = '3%';
            },
            levelMiddle: function() {
                this.level = '35%';
            },
            levelHiMiddle: function() {
                this.level = '60%';
            },
            levelHi: function() {
                this.level = '89%';
            }
        }
    }
    
    
</script>

<style lang="stylus" scoped>
    .leveljs
        width: 100%
        padding: 30px 0

    .leveljs__title
        width: 100%
        text-align: left
        font-size: 1.5em
        font-weight: 700
        line-height: 50px
        color: #2f1b15

    .leveljs__indicator
        width: 100%
        padding-top: 30px
        background-image: url("../assets/images/Horisontal.png")
        background-repeat: repeat no-repeat
        display: flex
        flex-wrap: wrap
        font-size: 13px
        font-weight: 700
        line-height: 20px
        color: #2f1b15
        position: relative

    progress
        appearance: none
        border: none
        width: 100%
        height: 0
        

    .marker
        width: 17px
        height: 30px
        background-image: url('../assets/images/Triangle.png') 
        background-repeat: no-repeat
        background-position: 0 80%
        position: absolute
        top: -5px
        transition: all ease .5s

    .first-part
        width: 20%
        padding-top: 30px
        background-image: url("../assets/images/Vertical_Long.png")
        background-repeat: no-repeat
        background-position: 0% 0
        padding-right: 10px
        cursor: pointer        

    .second-part
        width: 30%
        padding-top: 30px
        background-image: url("../assets/images/Vertical_Short.png")
        background-repeat: no-repeat
        background-position: -3% 0         
        padding-right: 10px
        cursor: pointer

    .third-part
        width: 27%
        padding-top: 30px
        background-image: url("../assets/images/Vertical_Short.png")
        background-repeat: no-repeat
        background-position: -3.5% 0      
        padding-right: 10px
        cursor: pointer

    .fourth-part
        width: 23%
        padding-top: 30px
        background-image: url("../assets/images/Vertical_Long.png")
        background-repeat: no-repeat
        background-position: 106.5% 0
        text-align: right                  
        padding-left: 10px
        cursor: pointer
        
</style>
