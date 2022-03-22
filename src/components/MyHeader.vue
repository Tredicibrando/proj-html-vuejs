<template>
    <header class="header">
        <MyJumbo />
    </header>
</template>
<script>


import MyJumbo from './MyJumbo.vue'


    export default {
        name: 'MyHeader',

        components: {
        MyJumbo,

        }   
    }

    
</script>

<style lang="scss" scoped>
.header{
    width: 100%;
    background-image: url(../assets/img/bg-6.jpg);
    min-height: calc(100vh - 33px);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: top;
}
</style>