<template>
    <div class="home_header">
        <div class="header-left">
            <span class="iconfont">&#xe624;</span>
        </div>
        <div class="header-center">
            <span class="iconfont">&#xe632;搜索热门景点</span>
        </div>
        <div class="header-right">
            城市<span class="iconfont">&#xe64a;</span>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Header'

}
</script>

<style lang="stylus" scoped>
    @import '../assets/styles/variables.styl'
    .home_header
        background $bgColor
        display flex
        line-height .86rem
        color #fff
        .header-left
            float left
            width .64rem
        .header-center
            border-radius .5rem
            margin-top .12rem
            margin-left .1rem
            background #ffffff
            height .64rem
            line-height .64rem
            flex 1
            color #ccc
        .header-right
            float right
            width 1.24rem
            text-align center
</style>
