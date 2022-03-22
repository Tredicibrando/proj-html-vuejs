<template>
    <section>
        <div class="container">
            <div class="services_wrapper">
                <h4 class="subtitle">
                    Our Business areas
                </h4>

                <h2 class="title">
                    Excellence in <span class="rect_decor">Services</span>
                </h2>

                <div class="text_wrapper">
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas nihil odit itaque praesentium at assumenda eos amet, recusandae maiores suscipit laborum consequatur illo consequuntur ab quam ipsam eius deserunt sit!
                    </p>
                    <input class="btn-green" type="button" value="See All">
                </div>
            </div>

            <div class="card_services_wrapper">
                <ServicesCard v-for="(element,i) in cardArray" :key="i" :element="element" />
            </div>
        </div>
    </section>
</template>

<script>

import ServicesCard from '@/components/ServicesCard.vue'
    export default {
        name:'MyServices',
        components:{
            ServicesCard,
        },
        data(){
            return{
                cardArray: [
                    {
                        img: require('../assets/img/network.svg'),
                        text: 'Audit & Assurance'
                    },

                    {
                        img: require('../assets/img/bag.svg'),
                        text: 'Financial Advisory'
                    },

                    {
                        img: require('../assets/img/charts.svg'),
                        text: 'Analytics and M&A'
                    },

                    {
                        img: require('../assets/img/plane.svg'),
                        text: 'Middle Marketing'
                    },

                    {
                        img: require('../assets/img/globe.svg'),
                        text: 'Legal Consulting'
                    },

                    {
                        img: require('../assets/img/box.svg'),
                        text: 'Regulatory Risk'
                    },
                ],
            }
        }

    }
</script>

<style lang="scss" scoped>
$lime: #EEF4ED;
$limed: #3d4955;

section{
    background-color: $lime;

    .container{
        width: 1240px;
        margin:  0 auto;
        padding: 35px 0;

        .services_wrapper{
            padding: 40px 0;
            color: $limed;

            .title{
                margin: 15px 0;
                font-size: 32px;
                font-weight: 800;

                .rect_decor{
                    background-color: rgba($color: #45bbbc, $alpha: 0.2) ;
                    padding: 5px 10px;
                    border-radius: 3px;
                    color: #45bbbc;
                }
            }

            .subtitle{
            color: #45bbbc;
            text-transform: uppercase;
            }

            .text_wrapper{
                margin-top: 25px;
                display: flex;
                justify-content: space-between;
                align-items: center;

                p{
                    width: 70%;
                }

                .btn-green{
                    padding: 10px 15px;
                    background-color: #22918e;
                    border: none;
                    text-transform: uppercase;
                    color: white;
                    border-radius: 3px;
                }
            }
        }

        .card_services_wrapper{
            padding: 20px 0;
            flex-wrap: wrap;
            display: flex;
            align-items: center;
            gap: 10px;
        }

    }
}
</style>