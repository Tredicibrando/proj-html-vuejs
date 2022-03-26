<template>
     <div class="card">
        <figure class="img_wrapper">
            <img src="../assets/img/team-1.jpg" alt="">
        </figure>
        <div class="text_wrapper">
            <h4 class="card_title">
             David Cooper
            </h4>
            <p class="card_subtitle">CTO and Co-Founder</p>

            <div class="icon_wrapper">
                <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                <a href="#"><i class="fa-brands fa-twitter"></i></a>
                <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
            </div>
        </div>
     </div>
</template>

<script>
    export default {
        name: 'ExpertCard',
        props:{
            element:{
                type: Object,
                require: true
            }
        },
        
    }
</script>

<style lang="scss" scoped>
.card{
    width: calc((100%/2) - 20px);
    display: flex;
    gap: 10px;

    .img_wrapper{
        width: max-content;
        border-radius: 3px;
        overflow: hidden;
        width: 85px;
        height: 120px;

        img{
            width: 100%;
            height: 100%;
            display: block;
            object-fit: cover;
        }
    }

    .text_wrapper{
        display: flex;
        flex-direction: column;
        color: white;

        .card_title{
            font-size: 24px;
            margin-bottom: 10px;
        }

        .card_subtitle{
            text-transform: uppercase;
            color: #ddd;
            margin-bottom: 10px;
            font-size: 12px;
        }

        .icon_wrapper{
            display: flex;
            gap: 5px;
            align-items: center;
            padding: 5px;
            color: #058283;
            margin-top: 10px;

            a{
                width: 30px;
                height: 30px;
                background-color: rgba($color: #058283, $alpha: 0.2);
                display: flex;
                justify-content: center;
                align-items: center;
                border-radius: 999px;
            }


        }
    }
}
</style>