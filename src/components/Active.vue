<template>
    <div>
        <section v-for="(item,index) in list" :key="index">
            <div class="top">
                <h5>{{item.msg}}</h5>
                <span>更多活动></span>
            </div>
            <div class="active">
                <img :src="item.src" alt="">
                <div class="gary">
                    <span>活动事件：2019.03.02~2019.10.17</span>
                    <span>进行中</span>
                </div>
            </div>
            <div>
                <span style="font-size: 14px">{{item.msg2}}</span>
            </div>
        </section>
    </div>
</template>

<script>
    export default {
        name: "Active",
        data(){
            return{
                list:[{
                    msg:"热门活动",
                    src:require("../assets/邀请好友banner.png"),
                    msg2:"场景活动-信用卡"
                },{
                    msg:"尊享专区",
                    src:require("../assets/抽奖banner.png"),
                    msg2:"注册参与抽奖好礼"
                }]
            }
        }
    }
</script>

<style scoped>
    *{
        margin: 0;
        padding: 0;
    }
    img{
        width: 400px;
    }
    .top{
        margin: 15px 0;
        width: 400px;
        display: flex;
        justify-content: space-between;
    }
    .top span{
        font-size: 13px;
        color: gray;
    }
    .top h5{
        border-left: 5px solid orange;
        padding-left: 5px;
    }
    .active{
        position: relative;
        width: 400px;
    }
    .gary{
        width: 400px;
        height: 40px;
        line-height: 40px;
        background-color: rgba(128, 128, 128, 0.3);
        font-size: 18px;
        color: white;
        display: flex;
        justify-content: space-around;
        position: absolute;
        bottom: 8px;
    }
</style>