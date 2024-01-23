<template>
  <h3>数据监听器</h3>
  <p >{{msg}}</p>
  <button @click="editMsg">修改数据</button>
</template>

<script>
export default {
  //属性
  data(){
    return {
      msg:"hello",
    }
  },

  //计算属性
  computed:{

  },

  //方法
  methods:{
    editMsg(){
      this.msg = "hello word"
    }
  },

  //监听
  watch:{
    //与data里面的属性一致
    msg(newVal,oldVal){
      //数据变化业务逻辑
      console.log(newVal,oldVal)
    }
  }
}
</script>

<style>
.active{
  font-size: 20px;
}
.text-danger{
  color: red;
  font-size: 30px;
}
</style>