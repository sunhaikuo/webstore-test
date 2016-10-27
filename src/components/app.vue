<script>
    import first from "./first"
    //es6
    export default {
        el:"#app",
        //data:function(){}，下面是es6写法
        data () {
            return {
                name:"guowenfh",
                age:"2q1"
            }
        },
        methods : {
            show() {
                alert(this.name);
            }
        },
        components : {first}
    }
</script>
<template>
    <div>
        <h1 @click="show">姓名：{{name}}</h1>
        <h2>{{age}}</h2>
    </div>
    <first ></first>
    <sec></sec>
</template>
<style  lang="less" rel="stylesheet/less">
    @import "../css/base";
    @bg-color:#899900;
    body{
        background-color: @bg-color;
    h1{
        background-color: #eee;
        color: red;
        transform: translate(10%, 10%);/*测试自动添加前缀*/
    }
    h1:hover{
        height:100px;
    }
    h2{
        background-color: #999;
    }
    }
</style>