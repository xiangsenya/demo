<template>
    <div>
        <div class="top">
            <h5>积分商城</h5>
            <span>更多商品></span>
        </div>
        <Box/>
    </div>
</template>

<script>
    import Box from "@/components/Box";

    export default {
        name: "Shop",
        components:{
            Box
        }
    }
</script>

<style scoped>
    *{
        margin: 0;
        padding: 0;
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
</style>