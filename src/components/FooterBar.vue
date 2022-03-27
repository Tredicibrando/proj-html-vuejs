<template>
    <div class="footer_bar">
        <div class="container">
            <p>Enjoy the low price. We are tracking any intention of piracy.</p>
            <p>© 2020 NEXTGEN is proudly Powered by <span class="green">Giovanni Nicolosi</span></p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'FooterBar'
    }
</script>

<style lang="scss" scoped>

.footer_bar{
    background-color: #0D0D11;
    padding: 20px;
    display: flex;
    align-items: center;
    margin-top: 100px;
    color: #ddd;

    .container{
        width: 1240px;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        padding: 7px 0;

        p{
            font-size: 14px;
        }

        .green{
            color: #45bbbc;
        }
    }
}

</style>