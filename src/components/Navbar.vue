<template>
    <div class="container">
        <div class="m">
            <ul class="leftPart">
                <li class="icon"><a href="javascript:;">Lantor微课</a></li>
                <template v-for="item in list" :key="item">
                    <li><a href="javascript:;">{{item}}</a></li>
                </template>
            </ul>
            <div class="centerPart">
                <i class="showTab"></i>
            </div>
            <div class="rightPart">
                <input type="text" placeholder="搜索关键字" class="search">
                <button class="login">注册登陆</button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name:'Navbar',
        props: [
            'list'
        ]
    }
</script>

<style lang="less" scoped>

    a {
        color: #999;
        text-decoration: none;
        &:hover {
            color: #777;
        }
    }

    .container {
        border-top: 2px solid #28a745;
        box-shadow: 0px 2px 1px 1px #eee;
        background-color: #fff;
        .m {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 56px;
            margin: 0 auto;

            .leftPart {
                flex: 10;
                display: flex;
                justify-content: space-between;
            }

            .centerPart {
                flex: 1;
                display: flex;
                justify-content: center;
                .showTab {
                    position: relative;
                    border: 1px solid #ccc;
                    border-radius: 5px;
                    display: none;
                    width: 24px;
                    height: 24px;
                    &::before {
                        position: absolute;
                        top: 50%;
                        left: 50%;
                        content: '';
                        width: 5px;
                        height: 5px;
                        border-top: 2px solid #ccc;
                        border-left: 2px solid #ccc;
                        transform: translate(-50%, -50%) rotate(-45deg);
                    }
                    &:hover {
                        background-color: #ccc;
                    }
                }
            }

            .rightPart {
                flex: 12;
                display: flex;
                align-items: center;
                .search {
                    height: 38px;
                    flex: 7;
                    border: 1px solid #ccc;
                    text-indent: 16px;
                    outline: none;
                    border-radius: 4px;
                    transition: .3s ease;
                    color: #333;
                    &:focus {
                        box-shadow: 0 0 3px 1px #28a745;
                        flex: 8;
                    }
                }

                .login {
                    box-sizing: border-box;
                    height: 40px;
                    flex: 3;
                    margin: 0 12px;
                    border: 1px solid #00965e;
                    border-radius: 5px;
                    cursor: pointer;
                    transition: .2s ease;
                    color: #fff;
                    background-color: #28a745;

                    &:hover {
                        background-color: #00965e;
                    }
                }
            }
        }
    }

</style>