<template>
    <div class="container">
        <div @click="buttonFunction">{{buttonText}}</div>
    </div>
</template>

<script>
export default {
    props:{
        buttonText:String,
        buttonFunction:Function
    }
}
</script>

<style scoped>
.container{
    padding: 5px 10px;
    background: var(--button-bg-color);
    border-radius: 4px;
}
</style>>