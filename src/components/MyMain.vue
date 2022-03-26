<template>
    <main>
        <MyCompany />
        <MyServices />
        <MyManagement />
        <MyExpert />
        <MyNews />
        <MyNewsletter />
    </main>
</template>

<script>
import MyCompany from '@/components/MyCompany.vue'
import MyServices from '@/components/MyServices.vue'
import MyManagement from '@/components/MyManagement.vue'
import MyExpert from '@/components/MyExpert.vue'
import MyNews from '@/components/MyNews.vue'
import MyNewsletter from '@/components/MyNewsletter.vue'

    export default {
        name:'MyMain',
        components:{
            MyCompany,
            MyServices,
            MyManagement,
            MyExpert,
            MyNews,
            MyNewsletter,

        }
    }
</script>

<style lang="scss" scoped>

</style>