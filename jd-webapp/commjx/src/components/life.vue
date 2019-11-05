<template>
    <div>
        <header>
            <p><img src="../assets/img/t01c18e525823affaf1_03.jpg"></p>
            <p><img src="../assets/img/t01c18e525823affaf1_05.jpg"></p>
            <p><img src="../assets/img/t01c18e525823affaf1_07.jpg"></p>
            <p><img src="../assets/img/t01c18e525823affaf1_09.jpg"></p>
        </header>
        <div class="nav">
            <p><a href="#/list?id='+index">{{list[0]}}</a></p><p><a href="#/phone?id='+index">{{list[1]}}</a></p><p><a href="#/voice?id='+index">{{list[2]}}</a></p><p><a href="#/equi?id='+index">{{list[3]}}</a></p><p><a href="#/life?id='+index">{{list[4]}}</a></p>
        </div>

    </div>
</template>

<script>
    export default {
        name: "vlife",
        data(){
            return {
                list:["推荐","手机","声学","配件","生活"],
                item:{}
            }
        }
    }
</script>

<style scoped>
    body,ul,ol,dl,dd,p,h1,h2,h3,h4,h5,h6,input,textarea,hr,div,em,strong{margin:0;padding:0;}
    body{font-family: "微软雅黑";}
    ul,ol{list-style-type: none;}
    a{text-decoration: none;}
    img{border: none;}
    clear：after{content:"";display:block;clear:both;height:0;overflow:hidden;visibility:hidden;}
    /*div {*/
    /*        font-size: 26.67vw;*/
    /*}*/
    div header{
        width: 100%;
        background-color: white;
        height: 0.26rem;
        display: flex;
        font-size: 0;
        margin-top: 0.1rem;
    }
    div header img{
        height: 0.26rem;
    }
    div header p:nth-child(1){
        margin-left: 0.2rem;
    }
    div header p:nth-child(2){
        margin-left: 1rem;
    }
    div header p:nth-child(3){
        margin-left:0.8rem;
    }
    div header p:nth-child(4){
        margin-left: 0.48rem;
    }
    div .nav{
        width: 100%;
        height: 0.36rem;
        display: flex;
        justify-content: space-around;
    }
    div .nav p{
        font-size: 0.16rem;
        height: 0.32rem;
        line-height: 0.32rem;
        font-weight: 500;

    }
    div.nav p a{
        color: black;
    }
    div .nav p:hover{
        border-bottom: 0.02rem solid cornflowerblue;
    }
    div .nav p:hover .nav p a{
        border-bottom: 0.02rem solid cornflowerblue;
        color: cornflowerblue;
    }
    div .banner{
        width: 100%;
        height: 2rem;
        margin-top: 0.1rem;
    }
    div .banner img{
        width: 100%;
        height: 100%;
    }
</style>