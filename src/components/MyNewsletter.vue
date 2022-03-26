<template>
    <section class="newsletter">
        <div class="container">
            <div class="row">
                <div class="col-50">
                    <h4>Newsletter</h4>
                    <h3><span>Know</span> First</h3>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nemo, vitae!</p>
                </div>
                <div class="col-50">

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
    padding: 100px 0; 
    background-image: url(../assets/img/bg-1.jpg);
    background-size: cover;
    background-position: center;

    .container{
        width: 1240px;
        margin: 0 auto;

        .row{
            display: flex;
            padding: 0 25px;

            .col-50{
                width: 50%;
            }
        }
    }
}
</style>