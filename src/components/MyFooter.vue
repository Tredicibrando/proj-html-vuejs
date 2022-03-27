<template>
    <footer class="footer">
        <div class="container">
            <div class="row">
                <div class="col-25">
                    <figure class="logo_wrapper">
                        <img src="../assets/img/nexgen-logo.svg" alt="">
                    </figure>
                    <p class="paragraph">
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Excepturi, consequatur?
                    </p>
                    <ul class="list_wrapper">
                        <li class="list_item">
                            <i class="fa-solid fa-phone"></i>
                            <a href="#">+1 (305) 1234-56789</a>
                        </li>
                        <li class="list_item">
                            <i class="fa-solid fa-envelope"></i>
                            <a href="#">hello@example.com</a>
                        </li>
                        <li class="list_item">
                            <i class="fa-solid fa-location-dot"></i>
                            <a href="#">Main Avenue, 987</a>
                        </li>
                    </ul>
                    <input class="footer-btn" type="button" value="Get in Touch">
                </div>
                <div class="right_footer">
                   <FooterCard />
                </div>
            </div>
        </div>

        <FooterBar />
    </footer>
</template>

<script>

import FooterBar from '@/components/FooterBar.vue'
import FooterCard from '@/components/FooterCard.vue'

    export default {
        name: 'MyFooter',
        components:{
            FooterBar,
            FooterCard,
        }
    }
</script>

<style lang="scss" scoped>
.footer{
    background-color: #111117;
    padding-top: 100px;
    color: white;
    display: flex;
    flex-direction: column;

    .container{
        width: 1240px;
        margin: 0 auto;

        .row{
            display: flex;
            gap: 25px;

            .col-25{
                width: 25%;

                .logo_wrapper{
                width: max-content;
                margin-bottom: 25px;

                    img{
                        width: 100px;
                
                    }

                }

               .paragraph{
                   margin-bottom: 25px;
                   color: #ddd;
                   font-size: 14px;
               }

                .list_wrapper{
                    display: flex;
                    flex-direction: column;
                    gap: 10px;
                    color: #ddd;
                    

                    .list_item{
                        display: flex;
                        gap: 10px;
                        align-items: center;
                    }
                }

                .footer-btn{
                    margin-top: 25px;
                    padding: 10px 15px;
                    border: 1px solid #058283;
                    color: white;
                    text-transform: uppercase;
                    background-color: transparent;
                    border-radius: 3px;
                }
            }

            .right_footer{
                width: 100%;
                display: flex;
                gap: 25px;
            }

           



        }
    }
}
</style>