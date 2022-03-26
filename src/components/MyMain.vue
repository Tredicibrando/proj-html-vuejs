<template>
    <main>
        <MyCompany />
        <MyServices />
        <MyManagement />
        <MyExpert />
    </main>
</template>

<script>
import MyCompany from '@/components/MyCompany.vue'
import MyServices from '@/components/MyServices.vue'
import MyManagement from '@/components/MyManagement.vue'
import MyExpert from '@/components/MyExpert'

    export default {
        name:'MyMain',
        components:{
            MyCompany,
            MyServices,
            MyManagement,
            MyExpert,

        }
    }
</script>

<style lang="scss" scoped>

</style>