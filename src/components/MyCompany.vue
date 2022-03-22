<template>
    <section class="company">
        <div class="container">
            <h4 class="subtitle">
                About the network
            </h4>


            <div class="row">
                <div class="col-50">
                    <h2 class="title">
                        <span class="rect_decor">The</span>
                        Company
                    </h2>

                    <p class="paragrafo">Lorem ipsum dolor sit amet consectetur adipisicing elit. Possimus, molestias!
                    Nihil vel hic ex magnam. Officiis non numquam ducimus repudiandae?
                    
                    Blanditiis eveniet laudantium reprehenderit a, nesciunt corporis magni aspernatur reiciendis.
                    Odit reiciendis blanditiis, placeat minus minima repudiandae. Porro, id modi!
                    Laudantium obcaecati eum totam iste sunt perspiciatis est esse cumque?
                    </p>
                    <br>
                    <p class="paragrafo">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde vero quo odio, rerum iusto repellat.
                    </p>
                </div>

                <div class="col-card">
                    <CompanyCard v-for="(element,i) in cardArray" :key="i" :element="element"/>
                </div>
            </div>
          
        </div>
    </section>
</template>

<script>
import CompanyCard from '@/components/CompanyCard.vue'

    export default {
        name: 'MyCompany',
        components:{
            CompanyCard,
        },

        data(){
            return{
                cardArray : [
                    {
                        img: require('../assets/img/medal.svg'),
                        text: 'Tradition'
                    },
                    {
                        img: require('../assets/img/security.svg'),
                        text: 'Security'
                    },
                    {
                        img: require('../assets/img/write.svg'),
                        text: 'Certificate'
                    },
                    {
                        img: require('../assets/img/laurea.svg'),
                        text: 'Expertise'
                    },
                ],
            }
        }
    }
</script>

<style lang="scss" scoped>

$fountain_blue: #45bbbc;

.company{
    background-color: #111117;
    padding: 40px 0;
}

.container{
    width: 1240px;
    margin: 0 auto;

    .subtitle{
        color: $fountain_blue;
        text-transform: uppercase;
        padding-bottom: 1.5rem;
    }

    .row{
        display: flex;
        width: 100%;
        align-items: center;

        .col-50{
            width: 50%;

            .title{
                color: white;
                font-size: 32px;
                padding-bottom: 1.5rem;
                font-weight: 800;

                .rect_decor{
                    background-color: rgba($color: #45bbbc, $alpha: 0.2) ;
                    padding: 5px 10px;
                    border-radius: 3px;
                }
            }

            .paragrafo{
                color: #ddd;
                font-size: 14px;
            }
        }
        
        .col-card{
            padding: 0 40px;
            width: 50%;
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }
    }
}
</style>