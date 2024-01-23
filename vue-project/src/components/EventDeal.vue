<template>
  <h3>事件处理</h3>
  <button @click="num++">按钮1</button>
  <button @click="num++">按钮1</button>
  <button @click="addNum">按钮2---{{num}}</button>
  <p>count={{num}}</p>
</template>

<script>
export default {
  //属性
  data(){
    return {
      num:0,
    }
  },
  //方法
  methods:{
    addNum()
    {
      this.num++
    }
  }
}
</script>