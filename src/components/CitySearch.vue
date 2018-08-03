<template>
    <div class="citySearch">
        <input class="citySearch-text" type="search" name="" placeholder="输入城市名称或拼音" id="">
    </div>
</template>

<script>
export default {
  name: 'CitySearch'
}
</script>

<style lang="stylus" scoped>
    @import '../assets/styles/variables.styl'
    .citySearch
        background $bgColor
        .citySearch-text
            border-radius .06rem
            margin .1rem auto
            width 99%
            text-align center
            padding 0 .1rem
</style>
