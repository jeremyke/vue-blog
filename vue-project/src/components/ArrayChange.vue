<template>
  <h3>数组变化的侦测</h3>
  <button @click="addListHandle">添加数据</button>
  <ul v-for="(num,index) of nameArr">
    <li :key="index">{{num}}</li>
  </ul>
</template>

<script>
export default {
  //属性
  data(){
    return {
      nameArr:["abc","def","ghi"],
    }
  },
  //方法
  methods:{
    addListHandle()
    {
      this.nameArr.push("jkl")
      console.log(this.nameArr)

      this.nameArr = this.nameArr.concat(["jkl"])
      console.log(this.nameArr)
    },
  }
}
</script>