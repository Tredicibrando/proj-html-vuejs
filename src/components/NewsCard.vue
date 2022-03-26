<template>
    <div class="card">

        <h3>
            {{element.text}}
        </h3>
    </div>
</template>

<script>
    export default {
        name: 'NewsCard',
        props:{
            element:{
                type: Object,
                require: true
            }
        }
    }
</script>

<style lang="scss" scoped>
    .card{
        width: calc((100% / 3 ) - 10px);
        background-color: black;
        height: 350px;
        background-size: cover;
        border-radius: 5px;
        display: flex;
        position: relative;
        overflow: hidden;
        justify-content: center;

        &::after{
            display: block;
            content: '';
            top: 0;
            right: 0;
            bottom: 0;
            left: 0;
            background-color: rgba($color: #131313, $alpha: 0.5);
            width: 100%;
            height: 100%;
            overflow: hidden;
        }

        h3{
            align-self: flex-end;
            text-align: center;
            color: white;
            position: absolute;
            padding: 35px 25px;
            font-size: 24px;
            width: 90%;
        }
    }
</style>