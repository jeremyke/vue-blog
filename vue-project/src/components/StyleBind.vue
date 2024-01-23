<template>
  <h3>style绑定</h3>
  <p :style="{color:colorVal,fontsize:fontsizeVal}">测试1</p>
  <p :style="[{color:colorVal,fontsize:fontsizeVal}]">测试2</p>

</template>

<script>
export default {
  //属性
  data(){
    return {
      colorVal:"red",
      fontsizeVal:"30px",
    }
  },

  //计算属性
  computed:{

  },

  //方法
  methods:{

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