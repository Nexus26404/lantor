<template>
    <div class="container">
        <navbar :list="list" class="navbar"></navbar>
        <div class="nothing"></div>
        <banner :picture="picSrc"></banner>
    </div>
</template>

<script>
    import Navbar from '@/components/Navbar.vue'
    import Banner from '@/components/Banner.vue'

    export default {
        name:'App',
        components: {
            Navbar,
            Banner
        },
        data(){
            return {
                picSrc: require('@/assets/logo.png'),
                list: ['课程', '问答', '专栏', '点评', '活动', '发现']
            }
        }
    }
</script>

<style lang="less" scoped>
    .container {
        width: 100%;
        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            z-index: 9999;
        }

        .nothing {
            height: 56px;
        }
    }
</style>