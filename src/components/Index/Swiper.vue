<template>
    <div class="swiper">
        <van-swipe class="my-swipe" :autoplay="3000" indicator-color="white">
            <van-swipe-item class="van-swipe-item">1</van-swipe-item>
            <van-swipe-item class="van-swipe-item">1</van-swipe-item>
        </van-swipe>
    </div>
</template>

<script>
    import { Swipe, SwipeItem } from 'vant'

    export default {
        name: "Swiper",
        components: {
            Swipe,
            SwipeItem
        }
    }
</script>

<style lang="less" scoped>
    .swiper {
        height: 150px;
        width: 300px;
        background-color: #39a9ed;
        overflow: hidden;
    }

    .my-swipe {
        display: block;
        color: #fff;
        font-size: 20px;
        line-height: 150px;
        height: 150px;
        text-align: center;
        background-color: #39a9ed;
        width: 300px;
        margin: 0 auto;
        overflow: hidden;

        .van-swipe-item {
            float: left;
            text-align: center;
            line-height: 150px;
            width: 300px;
        }
    }
</style>