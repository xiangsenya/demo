<template>
    <div class="total">
        <div class="content" v-for="(item,index) in list" :key="index">
            <img :src="item.src" alt="">
            <h6>{{item.msg}}</h6>
            <h6 style="color: orange">{{item.score}}积分</h6>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Box",
        data(){
            return{
                list:[{
                    src:require("../assets/积分-星巴克兑换券.png"),
                    msg:"星巴克5元兑换券",
                    score:"1000"
                },{
                    src:require("../assets/积分-爱奇艺会员.png"),
                    msg:"爱奇艺VIP会员卡",
                    score:"2000"
                },{
                    src:require("../assets/积分-芒果会员.png"),
                    msg:"芒果TV影视会员VIP年卡",
                    score:"1000"
                },{
                    src:require("../assets/积分-搜狐会员.png"),
                    msg:"搜狐VIP会员卡",
                    score:"2000"
                },]
            }
        }
    }
</script>

<style scoped>
    *{
        margin: 0;
        padding: 0;
    }
    .total{
        width: 400px;
        display: flex;
        flex-wrap: wrap;
    }
    .content{
        margin-left: 20px;
    }
    .content h6{
        margin: 10px;
    }
</style>