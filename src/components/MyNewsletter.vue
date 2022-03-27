<template>
    <section class="newsletter">
        <div class="container">
            <div class="row">
                <div class="col-50">
                    <h4 class="subtitle">Newsletter</h4>
                    <h3 class="title"><span class="rect_decor">Know</span> First</h3>
                    <p class="paragraph">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo, vitae!</p>
                </div>
                <div class="col-50">
                    <div class="input_wrapper">
                        <input class="input_text" type="text" placeholder="Name">
                        <input class="input_text" type="text" placeholder="Email">
                        <input class="input_button" type="button" value="subscribe">
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'MyNewsletter',

    }
</script>

<style lang="scss" scoped>
.newsletter{
    padding: 150px 0; 
    background-image: url(../assets/img/bg-1.jpg);
    background-size: cover;
    background-position: center;
    color: white;

    .container{
        width: 1240px;
        margin: 0 auto;

        .row{
            display: flex;
            padding: 0 35px;

            .col-50{
                width: 50%;

                .subtitle{
                    color: #45bbbc;
                    text-transform: uppercase;
                    margin-bottom: 25px;
                }

                .title{
                    font-size: 32px;
                    font-weight: 800;
                     margin-bottom: 25px;
                    
                    .rect_decor{
                    background-color: rgba($color: #45bbbc, $alpha: 0.2) ;
                    padding: 5px 10px;
                    border-radius: 3px;
                    color: white;
                    }
                }

                .paragraph{
                    color: #ddd;
                    font-size: 14px;
                }

                .input_wrapper{
                    display: flex;
                    flex-direction: column;
                    gap: 15px;

                    .input_text{
                        width: 400px;
                        padding: 10px 25px;
                        opacity: 0.5;
                        border-radius: 3px;
                        border: none;
                    }

                    .input_button{
                        padding: 10px 15px;
                        background-color: #22918e;
                        border: none;
                        text-transform: uppercase;
                        color: white;
                        border-radius: 3px;
                        width: 120px;
                        box-shadow: 0 0 15px rgb(19 19 19 / 10%);
                    }

                }



                
            }
        }
    }
}
</style>