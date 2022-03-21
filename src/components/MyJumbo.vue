<template>
    <div class="jumbo">
        <MyNav />


    </div>
</template>

<script>

import MyNav from '@/components/MyNav.vue'

    export default {
        name: 'MyJumbo',

        components:{
            MyNav
        }
    }
</script>

<style lang="scss" scoped>
    .jumbo{
        padding-top: 25px;
    }
</style>