<template>
    <header class="header">
        <MyBar />
        
    </header>
</template>

<script>

import MyBar from './MyBar.vue'

    export default {
        name: 'MyHeader',

        components: {
        MyBar,
        }   
    }

    
</script>

<style lang="scss" scoped>
.header{
    width: 100%;
    background-image: url(../assets/img/bg-6.jpg);
    min-height: calc(100vh - 40px);
    background-repeat: no-repeat;
    background-size: 100%;
}
</style>