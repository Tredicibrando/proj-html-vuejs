<template>
    <div class="card">
        <div class="icons_wrapper">
            <figure class="icon_wrapper">
                <img :src="element.img" alt="">
            </figure>

            <i class="fa-solid fa-arrow-right"></i>
        </div>

        <div class="text_wrapper">
            <h4 class="title">
                {{element.text}}
            </h4>

            <p class="subtitle">
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloremque sunt quibusdam quo repellat iste. Natus.
            </p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ServicesCard',
        props:{
            element:{
                type: Object,
                require: true
            }
        }
    }
</script>

<style lang="scss" scoped>

$limed: #3d4955;

.card{
    width: calc((100% - 20px) / 3);
    background-color: white;
    border-radius: 10px;
    padding: 25px 25px;
    box-shadow: 0 0 15px rgb(19 19 19 / 10%);

    .icons_wrapper{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;

        .icon_wrapper{
            width: max-content;
            
            img{
                width: 45px;
            }

            
        }

        i{
         font-size: 24px;
         color: #22918E;
         opacity: 0.7;
        } 
    }

    .text_wrapper{
        display: flex;
        flex-direction: column;
        gap: 5px;
        color: $limed;

        .title{
            font-weight: 800;
            font-size: 22px;
            margin-bottom: 10px;
        }
    }


}
</style>