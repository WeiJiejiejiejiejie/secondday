<template>
    <div>
    <div class="meizuPhone" :key="i" v-for="(n,i) in products">
        <p><img src="../../assets/img/q_03.jpg"/></p>
        <p>{{n.phonemodel}}</p>
        <p><span>{{n.dissprice}}</span>{{n.timeprice}}</p>
        <p>￥{{n.price}}</p>
    </div>

    </div>
</template>

<script>
    export default {
        name: "gitphotoa",
        data(){
            return {
                "products":[
                    {
                        "pic":"../../assets/img/q_03.jpg",
                        "phonemodel":"魅族 16S pro",
                        "dissprice":"新品",
                        "timeprice":"【限时领劵最高立减】",
                        "price":"2399"
                    },
                    {
                        "pic":"../../assets/img/q_10.jpg",
                        "phonemodel":"魅族 15S pro",
                        "dissprice":"直降",
                        "timeprice":"【限时领劵最高立减】",
                        "price":"2699"
                    },
                ]
            }
        }
    }
</script>

<style scoped>
    div .meizuPhone{
        width: 50%;
        font-size: 0.14rem;
        text-align: center;
        background-color: white;
    }
     div  .meizuPhone img {
        width: 96%;
        margin: 0 auto;
    }
     div .meizuPhone p:nth-child(3){
        border: 0.01rem solid red;
        width: 96%;
        margin: 0.1rem auto;
        color: red;
        overflow: hidden;

        text-overflow:ellipsis ;
        white-space: nowrap;
    }
     div .meizuPhone p:nth-child(3) span{
        background-color: red;
        width: 0.5rem;
        color: white;
        display: inline-block;
        float: left;
    }
     div .meizuPhone p:nth-child(4){
        color: red;
    }

</style>