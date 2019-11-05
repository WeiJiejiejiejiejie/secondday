<template>
    <div>
    <div class="meizuPhone" :key="i" v-for="(n,i) in products">
        <p><img src="../../assets/img/a_05.jpg"/></p>
        <p>{{n.phonemodel}}</p>
        <p style="border: none;color: #ccc;font-size: 0.12rem;">{{n.timeprice}}</p>
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
                        "pic":"../../assets/img/a_05.jpg.jpg",
                        "phonemodel":"MEIZU UR 高端定制耳机",
                        "dissprice":"新品",
                        "timeprice":"【预约专用】私人定制，为..",
                        "price":"200"
                    },
                    {
                        "pic":"../../assets/img/mmexport1571041220790_05.jpg",
                        "phonemodel":"魅族 EP3C 耳机",
                        "dissprice":"直降",
                        "timeprice":"Hi-res 认证高解析音质|高...",
                        "price":"129"
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