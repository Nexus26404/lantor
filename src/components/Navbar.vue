<template>
    <div class="container">
        <div class="m">
            <ul class="leftPart">
                <li><a href="javascript:;">Lantor微课</a></li>
                <li><a href="javascript:;">问答</a></li>
                <li><a href="javascript:;">专栏</a></li>
                <li><a href="javascript:;">课程</a></li>
                <li><a href="javascript:;">点评</a></li>
                <li><a href="javascript:;">活动</a></li>
                <li><a href="javascript:;">发现</a></li>
            </ul>
            <div class="rightPart">
                <input type="text" placeholder="搜索关键字" class="search">
                <button class="login">注册登陆</button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'Navbar'
    }
</script>

<style scoped>
    a {
        color: #999;
        text-decoration: none;
    }

    a:hover {
        color: #777;
    }

    .container {
        border-top: 2px solid #28a745;
        box-shadow: 2px 2px 1px 1px #eee;
    }

    .container .m {
        display: flex;
        justify-content: space-between;
        height: 56px;
        line-height: 56px;
        margin: 0 auto;
    }

    .container .leftPart li{
        list-style: none;
        float: left;
        margin-right: 30px;
        color: #999;
    }

    .container .rightPart .search {
        position: relative;
        top: -1px;
        height: 36px;
        width: 480px;
        border: 1px solid #ccc;
        text-indent: 16px;
        outline: none;
        border-radius: 4px;
        transition: .3s ease;
        color: #333;
    }

    .container .rightPart .search:focus {
        box-shadow: 0 0 3px 1px #28a745;
    }

    .container .rightPart .login {
        height: 36px;
        width: 100px;
        margin: 0 20px;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        transition: .2s ease;
        color: #fff;
        background-color: #28a745;
    }

    .container .rightPart .login:hover {
        background-color: #00965e;
    }
</style>