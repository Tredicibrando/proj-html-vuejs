<template>
    <div class="container">
        <ul class="navbar">

            <div class="logo_wrapper">
                <img src="../assets/img/nexgen-logo.svg" alt="">
            </div>

            <ul class="list_wrapper">
                <li v-for="(element,i) in navbar" :key="i" class="list_item">
                    <a href="href">{{element.item}}</a>
                </li>

                <input class="btn-green" type="button" value="Get in touch">
            </ul>

            

        </ul>
        
    </div>
</template>

<script>
    export default {
        name: 'MyNav',

        data(){
            return{
                navbar : [
                {
                    href: '#',
                    item:'Home'
                },
                {
                    href: '#',
                    item:'About'
                },
                {
                    href: '#',
                    item:'Services'
                },
                {
                    href: '#',
                    item:'Process'
                },
                {
                    href: '#',
                    item:'Team'
                },
                {
                    href: '#',
                    item:'Blog'
                },
            ]
            }
            
        }
    }
</script>

<style lang="scss" scoped>

$vibrant-green: #22918e;



     .navbar{
         display: flex;
         justify-content: space-between;
         align-items: center;

         .logo_wrapper{
             width: max-content;

             img{
                 height: 35px;
                 width: 100%;
             }
         }

         .list_wrapper{
             display: flex;
             align-items: center;
             gap: 15px;


             .list_item{
                 text-transform: uppercase;
             }

             .btn-green{
             padding: 10px 15px;
             background-color: $vibrant-green;
             border: none;
             text-transform: uppercase;
             color: white;
             border-radius: 3px;

            }
         }

         

     }
 
</style>