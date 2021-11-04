<template>
    <div>
        <tabbar></tabbar>
        <banner :picture="picSrc"></banner>
    </div>
</template>

<script>
    import Tabbar from '@/components/Tabbar.vue'
    import Banner from '@/components/Banner.vue'

    export default {
        name:'App',
        components: {
            Tabbar,
            Banner
        },
        data(){
            return {
                picSrc: require('@/assets/logo.png')
            }
        }
    }
</script>

<style scoped>
</style>