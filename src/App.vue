<template>
    <div class="container">
        <navbar :list="list" class="navbar"></navbar>
        <div class="nothing"></div>
        <index></index>
    </div>
</template>

<script>
    import Navbar from '@/components/Navbar.vue'
    import Index from '@/views/Index.vue'

    export default {
        name:'App',
        components: {
            Navbar,
            Index
        },
        data(){
            return {
                list: ['课程', '问答', '专栏', '点评', '活动', '发现']
            }
        }
    }
</script>

<style lang="less" scoped>
    @import url(./base/base.css);
    @import url(./common/css/style.css);

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