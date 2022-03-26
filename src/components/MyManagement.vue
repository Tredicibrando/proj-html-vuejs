<template>
    <section id="management">
        <div class="container_fluid">
            <div class="container">
                <div class="process">
                    <h4 class="subtitle">How it works in practice</h4>
                    <h3 class="title"><span class="rect_decor">Process</span> Management</h3>
                    <p class="paragraph">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Natus, corporis minus cumque doloribus nesciunt minima earum eaque pariatur consectetur? Iste porro incidunt laborum fuga dolor.</p>
                </div>
            </div>

            <div class="card_wrapper">
                <div class="card" v-for="(element,i) in cardArray" :key="i">
                    <div class="card_cerchio">{{element.number}}</div>
                    <h4 class="card_title">{{element.title}}</h4>
                    <p class="card_subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus, doloremque?</p>
                </div>
            </div>

            <div class="bar"></div>

        </div>
    </section> 
</template>

<script>
    export default {
        name: 'MyManagement',
        data(){
            return{
                cardArray: [
                    {
                        number: '1',
                        title: 'Collection of information',
                    },
                    {
                        number: '2',
                        title: 'Strategic planning',
                    },
                    {
                        number: '3',
                        title: 'Assignment of resposabilities',
                    },
                    {
                        number: '4',
                        title: 'Formatting process',
                    },
                    {
                        number: '5',
                        title: 'Continuity formalization',
                    },
                ],
            }
        }
        
    }
</script>

<style lang="scss" scoped>

$limed: #3d4955; 

    .container_fluid{
        width: 100%; 
        margin: 0 auto;
        padding: 100px 0;
        position: relative;

        .container{
            width: 1240px;
            margin: 0 auto;
            padding-bottom: 25px;

            .process{
                text-align: center;
                color: $limed;

                .title{
                    margin: 25px 0;
                    font-size: 32px;
                    font-weight: 800;
                    color: $limed;

                    .rect_decor{
                    background-color: rgba($color: #45bbbc, $alpha: 0.2) ;
                    padding: 5px 10px;
                    border-radius: 3px;
                    color: #058283;
                    }
                }

                .subtitle{
                    color: #45bbbc;
                    text-transform: uppercase;
                    font-size: 14px;
                    margin-bottom: 25px;
                    
                }

                .paragraph{
                    width: 70%;
                    margin: 0 auto;
                }

            }

        }

        .card_wrapper{
            display: flex;
            justify-content: center;
            align-items: center;
            margin-top: 30px;

           

            .card{
                width: calc((100% / 5) - 25px);
                display: flex;
                flex-direction: column;
                gap: 25px;
                justify-content: center;
                align-items: center;
                position: relative;

                .card_cerchio{
                    color: #058283;
                    font-weight: 800;
                    font-size: 18px;
                    z-index: 40;
                }

                .card_cerchio::after{
                    position: absolute;
                    display: block;
                    content: '';
                    width: 35px;
                    height: 35px;
                    background-color: #C2DFE0;
                    border-radius: 50%;
                    transform: translate(-50%,-50%);
                    top: 12px;
                    left: 50%;
                    z-index: -10;

                }

                .card_subtitle{
                    color: $limed;
                    text-align: center;
                }

                .card_title{
                    color: $limed;
                    font-size: 20px;
                    font-weight: 800px;
                }
            }

            
        }

        .bar::after{
            content: '';
            position: absolute;
            display: block;
            width: 100%;
            height: 3px;
            background-color: rgba($color: #45bbbc, $alpha: 0.2);
            left: 0;
            top: 58%;
        }

        


    }
</style>