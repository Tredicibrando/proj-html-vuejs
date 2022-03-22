<template>
    <div class="card">

        <div class="card_wrapper">
            <figure class="icon_wrapper">
                <img :src="element.img" alt="">
            </figure>  
            <h4>{{element.text}}</h4>
        </div>
        

        <p>Lorem ipsum dolor sit amet </p>
    </div>
</template>

<script>
    export default {
        name:'CompanyCard',
        props:{
            element:{
                type: Object,
                require: true
            }
        }
    }
</script>

<style lang="scss" scoped>
$limed: #22918E;
img{
    max-width: 100%;
}

.card{
    width: calc((100% - 30px) / 2);
    color: white;

    .card_wrapper{
        display: flex;
        align-items: center;
        justify-content: flex-start;
        margin-bottom: 1rem;
        

        .icon_wrapper{
            width: max-content;

            img{
                height: 25px;
                margin-right: 8px;
            }
        }

        
    }

    p{
            font-weight: 200;
            font-size: 14px;
    }
}
</style>