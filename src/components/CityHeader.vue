<template>
    <div class="cityHeader">
        <router-link to="/">
            <div class="cityHeader-left">
                <span class="iconfont">&#xe624;</span>
            </div>
        </router-link>
        <p class="cityTitle">城市选择</p>
    </div>

</template>

<script>
export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
    @import '../assets/styles/variables.styl'
    .cityHeader
        background $bgColor
        height .86rem
        display flex
        line-height .86rem
        .cityHeader-left
            color #ffffff
            float left
    .cityTitle
        text-align center
        margin 0 auto
        color #fff
        font-size .32rem
</style>
