<template>
    <section class="expert">
        <div class="container">
            <div class="row">
                <div class="col-70">
                    <div class="expert_team">
                        <h4 class="subtitle">
                            we like what we do
                        </h4>

                        <h3 class="title">
                            <span class="rect_decor">Team</span> of Experts
                        </h3>

                        <p class="paragraph">
                            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Alias facere illo qui eaque asperiores aperiam veniam sapiente at maiores quaerat!
                        </p>
                    </div>

                    <div class="card_wrapper">
                       <ExpertCard v-for="(element,i) in cardArray" :key="i" :element="element" />
                    </div>
                </div>

                <div class="col-30">
                    <div class="president">
                        <h4 class="president_title">
                            President Speech
                        </h4>
                        <p>
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus iste pariatur incidunt explicabo consequatur dolorum? Libero, dolorum! Quis omnis soluta placeat illo aliquam animi odit?
                        </p>
                        <br>
                        <p>
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus iste pariatur incidunt explicabo consequatur dolorum? Libero, dolorum! Quis omnis soluta placeat illo aliquam animi odit?
                        </p>
                        <br>
                        <p>
                            Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                        </p>
                        <br>
                        <h4 class="president_name">
                            T.Johnson
                        </h4>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import ExpertCard from '@/components/ExpertCard.vue'

    export default {
        name: 'MyExpert',
        components:{
            ExpertCard,
        },
        data(){
            return{
                cardArray: [
                    {
                        img: require('../assets/img/team-1.jpg'),
                        name: 'David Cooper',
                        role: 'Cto & Co-Founder'
                    },
                    {
                        img: require('../assets/img/team-3.jpg'),
                        name: 'Oliver Jones',
                        role: 'Chief Procurement'
                    },
                    {
                        img: require('../assets/img/team-2.jpg'),
                        name: 'Emma Lopez',
                        role: 'Chief Marketing'
                    },
                    {
                        img: require('../assets/img/team-4.jpg'),
                        name: 'T.Johnson',
                        role: 'CEO & President'
                    },

                ],
            }
        }
    }
</script>

<style lang="scss" scoped>
.expert{
    background-color: #111117;
    padding: 70px 0;

    .container{
        width: 1240px;
        margin: 0 auto;

        .row{
            display: flex;
            
            .col-70{
                width: 70%;

                .expert_team{
                    color: white;

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
                            padding: 5px 10px;
                            border-radius: 3px;
                        }
                        
                    }

                    .paragraph{
                        width: 90%;
                        margin-bottom: 35px;
                        color: #ddd;
                    }

                }

                .card_wrapper{
                    display: flex;
                    gap: 20px;
                    flex-wrap: wrap;
                }
            }

            .col-30{
                width: 30%;
                padding-left: 25px;

                .president{
                    margin-top: 25px;
                    border-radius: 3px;
                    background-color: #058283;
                    padding: 15px;
                    color: white;
                    height: max-content;
                    position: relative;

                    .president_title{
                        font-size: 18px;
                        margin-bottom: 10px;

                        
                    }

                    p{
                        color: #ddd;
                        font-size: 14px;
                    }

                    .president_name{
                        margin-top: 35px;
                    }

                    .president_name::after{
                        content: ' ”  ';
                        display: block;
                        font-size: 60px;
                        color: rgba($color: #055858, $alpha: 1.0);
                        position: absolute;
                        right: 20px;
                        bottom: -10px;
                        z-index: 40;
                    }
                }
            }
        }


    }


}
</style>