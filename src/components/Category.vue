<template>
    <div class="m category-box">
        <template v-for="item in cateList" :key="item.id">
            <category-item class="category-item" :listItem="item"></category-item>
        </template>
    </div>
</template>

<script>
    import CategoryItem from './CategoryItem.vue'

    export default {
        name: "Category",
        components: {
            CategoryItem
        },
        data(){
            return {
                cateList: [
                    {
                        id: 0,
                        icon: 'fire-o',
                        title: '专栏',
                        describe: '学习和分享技术知识'
                    },
                    {
                        id: 1,
                        icon: 'video-o',
                        title: '课程',
                        describe: '有计划提升专业技能'
                    },
                    {
                        id: 2,
                        icon: 'shop-collect-o',
                        title: '收藏',
                        describe: '收藏的视频'
                    },
                    {
                        id: 3,
                        icon: 'user-o',
                        title: '名师',
                        describe: '名校教师在线答疑'
                    }
                ]
            }
        }
    }
</script>

<style lang="less" scoped>
    .m {
        margin: 0 auto;
    }

    .category-box {
        display: flex;
        justify-content: space-around;
        .category-item {
            margin: 0 4px;
        }
    }
</style>