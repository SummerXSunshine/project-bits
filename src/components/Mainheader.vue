<template>
    <div class="wrap">
        <div class="container">
            <div class="title" v-for="(title, index) in headerTitleArr" :key="index">{{title}}</div>
            <div class="title-blank"></div>
            <div class="right-title"></div>
            <Button :button-text="colorMode" :button-function="changeColorMode"></Button>
        </div>
    </div>
</template>

<script>
import Button from './button'

export default {
    name:'header',
    props:['headerTitleArr'],
    components:{
        Button
    },
    data(){
        return {
            colorMode:'白天模式'
        }
    },
    methods:{
        changeColorMode(){
            console.log("sucess");
        }
    }
}
</script>

<style scoped>
.wrap{
    height: 52px;
    padding: 0 24px;
    background: var(--common-bg-color);
}
.container{
    margin: 0 auto;
    display: flex;
    align-items: center;
    font-size: 16px;
}
.title{
    padding: 15px 10px;
}
.title:hover{
    background-color: var(--select-bg-color);
}
.title-blank{
    display: flex;
    flex-grow: 1;
}
.right-title{
    
}
</style>>