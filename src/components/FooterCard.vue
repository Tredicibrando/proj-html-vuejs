<template>
<div class="footer-column">
     <div v-for="(element, i) in cardArray" :key="i" class="col-footer">
        <h3 class="footer_title">{{element.title}}</h3>
            <ul class="footer_list">
                <li v-for="(elemento,index) in element.items" :key="index" class="footer_item">
                    <i class="fa-solid fa-chevron-right"></i>
                    <a href="#">{{elemento.name}}</a>
                </li>
            </ul>
    </div>
</div>
    
</template>

<script>
    export default {
        name: 'FooterCard',
        data(){
            return{
                cardArray:[
                    {
                        title: 'About',
                        items:[
                            {
                                name: 'The Company',
                            },
                            {
                                name: 'Institutional',
                            },
                            {
                                name: 'Social & Events',
                            },
                            {
                                name: 'Innovation',
                            },
                            {
                                name: 'Environment',
                            },
                            {
                                name: 'Technology',
                            },
                        ],
                    },
                    {
                        title: 'Services',
                        items:[
                            {
                                name: 'Audit & Assurance',
                            },
                            {
                                name: 'Financial Advisory',
                            },
                            {
                                name: 'Analytics M&A',
                            },
                            {
                                name: 'Middle Marketing',
                            },
                            {
                                name: 'Legal Consulting',
                            },
                            {
                                name: 'Regulatory Risk',
                            },
                        ],
                    },
                     {
                        title: 'Support',
                        items:[
                            {
                                name: 'Responsability',
                            },
                            {
                                name: 'Terms of Use',
                            },
                            {
                                name: 'Privacy Policy',
                            },
                            {
                                name: 'About Cookies',
                            },
                            {
                                name: 'Accessibility',
                            },
                            {
                                name: 'Information',
                            },
                        ],
                    },
                ],
            }
        }
    }
</script>

<style lang="scss" scoped>
.footer-column{
    display: contents;

    .col-footer{
    width: calc((100% / 3 ) - 10px);
    background-color: rgba($color: #ffffff, $alpha: 0.1);
    border-radius: 5px;
    padding: 25px;

    .footer_title{
        margin-bottom: 25px;
    }

    .footer_list{
        display: flex;
        flex-direction: column;
        gap: 5px;

     .footer_item{
         display: flex;
         gap: 5px;
         align-items: center;
         color: #ddd;
         margin-bottom: 5px;

         i{
             font-size: 14px;
         }
     }
    }
} 
}

 

</style>