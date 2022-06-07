<template>
    <div class="total">
        <div class="box" v-for="(item,index) in list" :key="index" v-if="index<2">
            <div class="top">
                <img style="width: 100px" :src="item.src" alt="">
            </div>
            <div class="bottom">
                <h5>{{item.name}}</h5>
                <span style="font-size:16px">{{item.type}}|{{item.address}}</span>
                <p style="font-size: 16px;color: gray"><img style="width: 16px" :src="item.src2" alt="">89购100元代金券</p>
                <p style="font-size: 16px;color: gray"><img style="width: 16px" :src="item.src2" alt="">89购100元代金券</p>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "AreaDetail",
        data(){
            return{
                list:[{
                    src:require("../assets/商户占位图01@2x.png"),
                    src2:require("../assets/icon_券@2x.png"),
                    name:"麦当劳(武昌火车站)",
                    type:"快餐",
                    address:"玉林公园"
                },{
                    src:require("../assets/商户占位图02@2x.png"),
                    src2:require("../assets/icon_券@2x.png"),
                    name:"蛙来哒(万达广场)",
                    type:"中餐",
                    address:"万达广场"
                },{
                    src:require("../assets/商户占位图03@2x.png"),
                    src2:require("../assets/icon_券@2x.png"),
                    name:"肯德基(武昌火车站)",
                    type:"快餐",
                    address:"玉林公园"
                },{
                    src:require("../assets/商户占位图04@2x.png"),
                    src2:require("../assets/icon_券@2x.png"),
                    name:"星巴克(K11)",
                    type:"快餐",
                    address:"玉林公园"
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
    .box{
        width: 400px;
        display: flex;
        justify-content: space-around;
    }
</style>