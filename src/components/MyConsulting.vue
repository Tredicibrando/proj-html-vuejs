<template>
    <div class="consulting">
        <div class="consulting_wrapper">
            <h4 class="subtitle">Fusions & aquisitions</h4>
            <h1 class="title">Insurance Consulting</h1>

            <div class="input_wrapper">
                <input class="input_text" type="text" placeholder="Name">
                <input class="input_text" type="text" placeholder="Email">
                <input class="input_text" type="text" placeholder="Phone">
                <input class="input_text" type="text" placeholder="More Info">
                <i class="fa-solid fa-chevron-down"></i>
            </div>

            <input class="btn-green" type="button" value="Get in touch">
            <input class="btn-white" type="button" value="Read More">
        </div>
    </div>
</template>

<script>
    export default {
        name: 'MyConsulting'
    }
</script>

<style lang="scss" scoped>

$vibrant-green: #22918e;
$fountain_blue: #45bbbc;
$limed: #3d4955;
$black_haze: #CED2D5;

.consulting{
    padding-top: 5rem;
    display: flex;
    justify-content: flex-end;
    

    .consulting_wrapper{
        width: 50%;
        padding-left: 7rem;

        .subtitle{
            font-size: 16px;
            color: #0EA7AB;
            font-weight: 600;
            text-transform: uppercase;
        }

        .title{
            font-size: 54px;
            width: 90%;
            font-weight: 900;
            color: $limed;
            padding-bottom: 20px;
        }

        .input_wrapper{
            display: flex;
            gap: 8px;
            width: 100%;
            flex-wrap: wrap;
            position: relative;
            padding-bottom: 15px;

            .input_text{
            background-color:  $black_haze;
            padding: 12px 15px;
            border: none;
            border-radius: 3px;
            width: calc((100% /2) - 8px);
            }


            

        }

        .fa-chevron-down{
            position: absolute;
            right: 10px;
            top: 65%;
            transform: translate(-50%,-50%);
            color: $limed;
            font-size: 12px;
        }

        .btn-green{
             padding: 10px 15px;
             background-color: $vibrant-green;
             border: none;
             text-transform: uppercase;
             color: white;
             border-radius: 3px;

        }

        .btn-white{
             padding: 10px 15px;
             background-color: transparent;
             border: 1px solid $vibrant-green;
             text-transform: uppercase;
             color: $vibrant-green;
             border-radius: 3px;
             margin-left: 15px;

        }
          
        
    }



}
</style>