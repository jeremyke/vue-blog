<template>
  <h3>组件生命周期的应用</h3>
  <p ref="name">哈哈哈</p>
  <ul>
    <li v-for="(item,index) of banner" :key="index">
      <h4>{{item.title}}</h4>
      <p>{{item.content}}</p>
    </li>
  </ul>
</template>

<script>
export default {
  name: "UseComponent",
  mounted() {
    console.log(this.$refs.name)
  },
  created() {
    this.banner = [
      {
        title: "我是",
        content:"我是我是我是我是我是我是我是我是我是我是我是我是"
      },
      {
        title: "你是",
        content:"我是我是我是我是我是我是我是我是我是我是我是我是"
      },
      {
        title: "他是",
        content:"我是我是我是我是我是我是我是我是我是我是我是我是"
      }
    ]
  },
  data(){
    return{
      banner:[],
    }
  }
}
</script>


<style scoped>

</style>