<template>
  <h3>事件修饰符</h3>

  <a href="http://baidu.com" @click.prevent="clickHandle">百度</a>

  <div @click="clickDiv">
    <p @click.stop="clickP">冒泡</p>
  </div>

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
    clickHandle()
    {
      console.log("点击了")
    },
    clickDiv()
    {
      console.log("点击了clickDiv")
    },
    clickP()
    {
      console.log("点击了clickP")
    },
  }
}
</script>