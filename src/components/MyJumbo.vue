<template>
<div class="jumbo">
    <div class="container">
        <MyNav />  
        <MyConsulting />
    </div>
</div>   
</template>

<script>

import MyNav from '@/components/MyNav.vue'
import MyConsulting from '@/components/MyConsulting.vue'

    export default {
        name: 'MyJumbo',

        components:{
            MyNav,
            MyConsulting,
        }
    }
</script>

<style lang="scss" scoped>
    .jumbo{
        padding-top: 25px;

        .container{
        width: 1240px;
        margin: 0 auto;
        } 
    }
</style>