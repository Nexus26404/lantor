<template>
    <div class="index">
        <banner :picture="picSrc"></banner>
        <article class="home-content m">
            <category class="category"></category>
            <swiper></swiper>
        </article>
    </div>
</template>

<script>
    import Banner from '@/components/Index/Banner.vue'
    import Category from '@/components/Index/Category.vue'
    import Swiper from '@/components/Index/Swiper.vue'

    export default {
        name: "Index",
        components: {
            Banner,
            Category,
            Swiper
        },
        data(){
            return {
                picSrc: require('@/common/img/bg.jpg')
            }
        }
    }
</script>

<style lang="less" scoped>
    .category {
        position: relative;
        top: -60px;
    }

    .m {
        margin: 0 auto;
    }

    .home-content {
        height: 100vh;
        background-color: pink;
    }

</style>