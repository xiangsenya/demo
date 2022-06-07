<template>
    <div class="total">
        <div class="box" v-for="(item,index) in list" :key="index">
            <img :src="item.src" alt="">
            <span>{{item.msg}}</span>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Icon",
        data() {
            return {
                list:[
                    {
                        src:require("../assets/icon_签到.png"),
                        msg: "签到有礼"
                    },
                    {
                        src:require("../assets/icon_邀请.png"),
                        msg: "邀请有礼"
                    },
                    {
                        src:require("../assets/icon_会员.png"),
                        msg: "会员专享"
                    },
                    {
                        src:require("../assets/编组 6.png"),
                        msg: "任务专区"
                    }
                ]
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
        flex-wrap: nowrap;
        justify-content: space-around;
    }
    .box{
        display: flex;
        flex-direction: column;
        align-content: center;
    }
    .box span{
        font-size: 12px;
    }
    .box img{
        width: 40px;
        height: 40px;
    }
</style>