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

                    <div class="card-wrapper">
                       <ExpertCard :element="element" />
                    </div>
                </div>
                <div class="col-30">

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
                        img: require('../assets/img/team-2.jpg'),
                        name: 'Oliver Jones',
                        role: 'Chief Procurement'
                    },
                    {
                        img: require('../assets/img/team-3.jpg'),
                        name: 'David Cooper',
                        role: 'Cto & Co-Founder'
                    },
                    {
                        img: require('../assets/img/team-4.jpg'),
                        name: 'David Cooper',
                        role: 'Cto & Co-Founder'
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
                    }

                }

                .card_wrapper{
                    display: flex;
                    gap: 20px;
                }
            }

            .col-30{
                width: 30%;
            }
        }


    }


}
</style>