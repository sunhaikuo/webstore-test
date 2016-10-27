<script>
    export default {
        data() {
            return {
                name : "tet"
            }
        },
        methods : {
            test : function () {
//                getMyName();
                this.name = "sunhakikuo"
            }
        }
    }
</script>
<template>
	<button class="my-btn" @click="test">Click to show your name</button>
	<p>{{name}}</p>
    <a href="#" class="logo">

    </a>
</template>
<style lang="less" rel="stylesheet/less">
    @import "../css/base";
    @fs:20px;
    .my-btn{
        font-size: @fs;
        color: @my-color;
    }
    p {
        font-size: @fs;
        color: yellow;
    }
    .logo {
        display: block;
        width:270px;
        height:129px;
        background: url("/src/img/logo_white.png");
        background-size: 100%  100%;
    }
</style>