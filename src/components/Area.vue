<template>
    <div>
        <div>
            <div class="top">
                <h5>营口专区</h5>
                <span>更多商户></span>
            </div>
            <AreaDetail/>
        </div>
    </div>
</template>

<script>
    import AreaDetail from "@/components/AreaDetail";

    export default {
        name: "Area",
        components:{
            AreaDetail
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