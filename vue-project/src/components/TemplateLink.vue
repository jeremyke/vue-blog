<template>
  <h3>模版引用</h3>
  <div ref="container" class="container">{{content}}</div>
  <button @click="getEleHandle">获取元素</button>


</template>

<script>
//1. 内容修改使用{{}} 2.属性改变使用v-bind:指令 3.事件v-on:事件
export default {
  //属性
  data(){
    return {
      content:"内容",
    }
  },

  //计算属性
  computed:{

  },

  //方法
  methods:{
    getEleHandle(){
      console.log(this.$refs.container)
      this.$refs.container.innerHTML = "xxxx"
    }
  },

  //监听
  watch:{

  }
}
</script>

<style>

</style>