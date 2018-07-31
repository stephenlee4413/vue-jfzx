<template>
    <div id="todos">
        <b-form-input v-model="inputValue" />
        <b-button v-on:click="handleAdd" style="heigth:12px;magrin-left:10px;">添加</b-button>
        <b-list-group>
            <b-list-group-item v-for="(item,index) of content" :key="index">
                <div>
                    <b-card :title="pushTime" img-src="https://picsum.photos/600/300/?image=25" img-alt="Image" img-top tag="article" style="max-width: 20rem;" class="mb-2">
                        <p class="card-text">
                            {{item}}
                        </p>
                        <b-button class="styTest" href="#" variant="primary">查看详情</b-button>
                    </b-card>
                </div>
            </b-list-group-item>
        </b-list-group>
    </div>
</template>

<script>
export default {
  name: 'Todos',
  data () {
    return {
      content: [],
      inputValue: '',
      pushTime: new Date().toLocaleString()
    }
  },
  methods: {
    handleAdd () {
      // this.$data.content.push()
      // console.log(this.inputValue);
      this.$data.content.push(this.inputValue)
      this.inputValue = ''
    }
  }
}
</script>

// 样式部分
<style lang="stylus" scoped>

</style>
