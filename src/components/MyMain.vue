<template>
    <main>
        <MyCompany />
        <MyServices />
    </main>
</template>

<script>
import MyCompany from '@/components/MyCompany.vue'
import MyServices from '@/components/MyServices.vue'

    export default {
        name:'MyMain',
        components:{
            MyCompany,
            MyServices,
        }
    }
</script>

<style lang="scss" scoped>

</style>