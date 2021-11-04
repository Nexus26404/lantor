<template>
    <div class="bg" :style="{ background: 'url(' + picture + ') no-repeat center top', backgroundSize: 'cover' }">
        <!-- <img :src="picture"> -->
    </div>
</template>

<script>
    export default {
        name: "Banner",
        props: [
            "picture"
        ]
    }
</script>

<style lang="less" scoped>
    .bg {
        width: 100%;
        height: 45vh;
        overflow: hidden;
        img {
            width: 100%;
        }
    }
</style>