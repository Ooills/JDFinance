<template lang="html">
    <div :class="$style.header">
        <span :class="$style.left">
            <a href="www.qq.com" class="regist">注册</a>&nbsp;|&nbsp;<a href="www.baidu.com" class="login">登录</a>
        </span>
        <btn :class="$style.btnDownLoad">APP下载</btn>
    </div>
</template>

<script>
    import btn from "../core/btn"
    export default {
        components: {
            btn
        }
    }
</script>

<style module lang="scss">
    .header{
        color: #666;
        height: 100px;
        line-height: 100px;
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        font-size: 32px;
        background: #fff url(//m.jr.jd.com/spe/qyy/main/images/jr-logo.png) center center no-repeat;
        background-size: auto 50%;
        z-index: 100;
        .left{
            font-size: 28px;
            height: 30px;
            line-height: 30px;
            margin: 17px 0 0 18px;
        }
        .btnDownLoad{
            font-size: 24px;
            height: 48px;
            line-height: 48px;
            float: right;
            border: 0;
            min-width: 120px;
            border-radius: 4px;
            text-align: center;
            margin: 28px 28px 0 0;
        }
    }
</style>