<template>
    <nav class="fixed_bar">
        <div class="container">
            <div class="row">
                <div class="hour">
                    <i class="fa-solid fa-clock"></i>
                    <p> Open Hours: Mon - Sat 9:00 - 18:00</p>
                </div>

                <div class="info">
                    <i class="fa-solid fa-phone"></i>
                    <p>+1 (305) 1234 5678</p>
                    <i class="fa-solid fa-envelope"></i>
                    <p>hello@example.com</p>

                    <div class="social">
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-linkedin-in"></i>
                    </div>
                </div>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        name: 'MyBar'
    }
</script>

<style lang="scss" scoped>

$limed: #3d4955;

.fixed_bar{
    background-color: $limed;
    width: 100%;
    color: white;

    .container{
        width: 1240px;
        margin: 0 auto;

        .row{
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 7px 0;
            font-weight: 200;

            i{
                font-size: 14px;
                opacity: 70%;

                &:hover{
                    opacity: 100%;
                }
            }

            

            .hour{
                display: flex;
                align-items: center;
                gap: 5px;



            }

            .info{
                display: flex;
                align-items: center;
                gap: 10px;

                .fa-phone, 
                .fa-envelope{
                    margin-right: 10px;
                    margin-left: 10px;
                }

                .social{
                    display: flex;
                    align-items: center;
                    gap: 15px;
                    margin-left: 10px;
                    
                }
            }
        }
    }
}

</style>