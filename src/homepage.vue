<template>
    <MainHeader :headerTitleArr='headerTitle'></MainHeader>
</template>

<script>
import MainHeader from './components/Mainheader.vue'

export default {
    components:{
        MainHeader
    },
    data(){
        return{
            headerTitle:['home','books','movies','notes']
        }
    },
}
</script>