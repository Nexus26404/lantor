<template>
    <div class="list-container">
        <div class="category-left">
            <van-icon :name="listItem.icon" size="24px" color="#00965e" />
        </div>
        <div class="category-right">
            <h3>{{listItem.title}}</h3>
            <p class="category-intro">{{listItem.describe}}</p>
        </div>
    </div>
</template>

<script>
    import { Icon } from 'vant'
    import 'vant/es/icon/style'

    export default {
        name: "CategoryItem",
        components: {
            VanIcon: Icon
        },
        props: [
            'listItem'
        ]
    }
</script>

<style lang="less" scoped>
    .list-container {
        width: 240px;
        height: 120px;
        background-color: #fff;
        border-radius: 10px;
        display: flex;
        justify-content: center;
        align-items: center;
        box-shadow: 0 1px 2px 1px #ccc;
        .category-left {
            flex: 1;
            display: flex;
            justify-content: center;
        }
        .category-right {
            flex: 3;
            display: flex;
            flex-direction: column;
            align-items: flex-start;
            .category-intro {
                font-size: 14px;
            }
        }
    }
</style>