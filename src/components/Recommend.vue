<template>
    <div>
        <div class="recommend-title">
            <p class="title-text">热销推荐</p>
        </div>
        <ul v-for="item of recommendList" :key="item.id">
            <li class="item">
                <div class="item-img-wrapper">
                    <img class="item-img" :src="item.imgUrl" alt="">
                </div>
                <div class="item-info">
                    <p class="item-title">{{item.title}}</p>
                    <p class="item-desc">{{item.desc}}</p>
                    <button class="item-btn">查看详情</button>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
  name: 'Recommend',
  data () {
    return {
      recommendList: [{
        id: '001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201403/03/77a8f60ea243465fdf2c937e2edd33dd.jpg_200x200_51dd1e90.jpg',
        title: '国色天乡海洋公园',
        desc: '在成都市温江区有一个地方叫国色天乡，碰碰车,西红柿首富，中国共产党人民解放军，八一建军节，军人的荣耀。'
      },
      {
        id: '002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201403/03/77a8f60ea243465fdf2c937e2edd33dd.jpg_200x200_51dd1e90.jpg',
        title: '国色天乡海洋公园',
        desc: '在成都市温江区有一个地方叫国色天乡，碰碰车,西红柿首富，中国共产党人民解放军，八一建军节，军人的荣耀。'
      }, {
        id: '003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/201403/03/77a8f60ea243465fdf2c937e2edd33dd.jpg_200x200_51dd1e90.jpg',
        title: '国色天乡海洋公园',
        desc: '在成都市温江区有一个地方叫国色天乡，碰碰车,西红柿首富，中国共产党人民解放军，八一建军节，军人的荣耀。'
      }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
    @import '../assets/styles/variables.styl'
    .recommend-title
        width 100%
        background #00bcd4
        line-height .6rem
        color white
        text-indent .2rem
    .item
        display flex
        overflow hidden
        height 1.8rem
        .item-img
            height 1.9rem
            width 1.9rem
            padding .1rem
        .item-info
            flex 1
            min-width 0
            // padding .1rem
            .item-title
                line-height .6rem
                font-size .3rem
                padding-top 0
                float left
                ellipsis()
            .item-desc
                float left
                width 100%
                text-align justify
                height .76rem
                overflow hidden
                text-overflow ellipsis
                color #ccc
            .item-btn
                float left
                height .4rem
                margin-bottom .1rem
                margin-top .1rem
                background #ff9300
                border-radius .1rem
</style>
