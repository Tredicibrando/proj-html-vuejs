<template>
    <section>
        <div class="container">
            <div class="editorial">
                <h4 class="subtitle">Our Editorial content</h4>
                <h3 class="title">Latest <span class="rect_decor">News</span></h3>
                <div class="text_wrapper">
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ex, odio facere iusto reprehenderit nemo minima!</p>
                    <input type="button" value="See All">
                </div>
            </div>

            <div class="card_wrapper">
                <NewsCard v-for="(element,i) in cardArray" 
                :key="i" 
                :style="`background-image: url(${element.img})`"
                :element="element" />
            </div>
        </div>
    </section>
</template>

<script>
import NewsCard from '@/components/NewsCard.vue'

    export default {
        name: 'MyNews',
        components:{
            NewsCard,
        },
        data(){
            return{
                cardArray: [
                    {
                        img: require('../assets/img/news-1.jpg'),
                        text: 'Incresing creativity is possible for everyone'
                    },
                    {
                        img: require('../assets/img/news-2.jpg'),
                        text: 'Because market research is part of the business plan'
                    },
                    {
                        img: require('../assets/img/news-3.jpg'),
                        text: 'Working from home is now a trend'
                    },
                ],
            }
        }

    }
</script>

<style lang="scss" scoped>

$limed: #3d4955;


.container{
    width: 1240px;
    margin: 0 auto;
    padding: 60px 0;

    .editorial{
        color: $limed;

        .subtitle{
            color: #058283;
            text-transform: uppercase;
            margin-bottom: 25px;
        }

        .title{
            font-weight: 800;
            font-size: 32px;
            margin-bottom: 25px;

            .rect_decor{
                background-color: rgba($color: #058283, $alpha: 0.2);
                border-radius: 3px;
                padding: 5px 10px;
                color: #058283;
            }
        }
        
        .text_wrapper{
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 35px;

            input{
                padding: 10px 15px;
                background-color: #22918e;
                border: none;
                text-transform: uppercase;
                color: white;
                border-radius: 3px;
            }
        }

    }

    .card_wrapper{
        display: flex;
        justify-content: space-between;
    }


}
</style>