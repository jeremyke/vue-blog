<template>
  <h3>事件传参</h3>
  <button @click="addNum">按钮</button>
  <button @click="printNum('hello',$event)">按钮传参</button>
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
    //获取event对象
    addNum(e)
    {
      console.log(e)
      e.target.innerHTML = "ADD" + this.num
      this.num++
    },
    //传参（参数放前，e放在后面）
    printNum(param,e)
    {
      console.log(param)
      e.target.innerHTML = "print " + param
    }
  }
}
</script>