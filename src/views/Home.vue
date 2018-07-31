<template>
  <div class="home">
    <home-header></home-header>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
// 引入header区域内容
import HomeHeader from '@/components/Header.vue'

export default {
  name: 'home',
  components: {
    HomeHeader
  }
}
</script>
