<template>
    <div>
        <img src="../assets/返回.png" alt="">
        <h3>{{msg}}</h3>
        <img src="../assets/更多.png" alt="">
    </div>
</template>

<script>
    export default {
        name: "Head",
        data(){
            return{
                msg:"营口银行"
            }
        }
    }
</script>

<style scoped>
    *{
        margin: 0;
        padding: 0;
    }
    div{
        width: 400px;
        display: flex;
        justify-content: space-around;
    }

</style>