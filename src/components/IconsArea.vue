<template>
    <div class="iconsArea">
        <div
        class="icon"
        v-for="item of iconList"
        :key="item.id">
            <div class="icon-img">
                <img class="icon-content" :src="item.imgUrl" alt="">
                <p class="icon-text">{{item.describe }}</p>
            </div>
        </div>
        <!-- <div class="icon"></div>
            <div class="icon"></div>
            <div class="icon"></div>
            <div class="icon"></div>
            <div class="icon"></div>
            <div class="icon"></div>
            <div class="icon"></div> -->
    </div>
</template>

<script>
export default {
  name: 'IconsArea',
  data () {
    return {
      iconList: [
        {
          id: '001',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/f3dd6c383aeb3b02.png',
          describe: '热门景点'
        },
        {
          id: '002',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/3e/86314b2af03b7502.png',
          describe: '热门景点'
        },
        {
          id: '003',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/ff/fdf170ee89594b02.png',
          describe: '热门景点'
        }, {
          id: '004',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/95/8d02011d149bdb02.png',
          describe: '热门景点'
        },
        {
          id: '005',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/50/26ffa31b56646402.png',
          describe: '亲子游'
        },
        {
          id: '006',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/50/26ffa31b56646402.png',
          describe: '海洋馆'
        }, {
          id: '007',
          describe: '一日游',
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1804/5a/13ceb38dcf262f02.png'
        }, {
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/8246f27355943202.png',
          id: '008',
          describe: '游乐场'
        }, {
          imgUrl: 'http://img1.qunarzz.com/piao/fusion/1803/95/8246f27355943202.png',
          id: '009',
          describe: '城市游'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
    @import '../assets/styles/variables.styl'
    .iconsArea
        overflow hidden
        height 0
        padding-bottom 50%
        .icon
            position relative
            overflow hidden
            float left
            width 25%
            padding-bottom 25%
            .icon-img
                position absolute
                bottom .44rem
                top 0
                left 0
                right 0
                box-sizing border-box
                padding .1rem
                .icon-content
                    height 100%
                    display block
                    margin 0 auto
            .icon-text
                position absolute
                bottom 0
                left 0
                right 0
                height .44rem
                line-height .44rem
                text-align center
                color $darkTextColor
                padding-top .24rem

</style>
