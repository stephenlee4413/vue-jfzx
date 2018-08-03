<template>
  <div class="home">
    <home-header></home-header>
    <!-- <home-swiper></home-swiper> -->
    <home-icons></home-icons>
    <home-recommend></home-recommend>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
// 引入header区域内容
import HomeHeader from '@/components/Header.vue'
// 引入swiper组件
// import HomeSwiper from '@/components/Swiper.vue'
import HomeIcons from '@/components/IconsArea.vue'

import HomeRecommend from '@/components/Recommend.vue'

export default {
  name: 'home',
  components: {
    HomeHeader,
    // HomeSwiper,
    HomeIcons,
    HomeRecommend
  }
}
</script>
