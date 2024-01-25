<template>
  <h3>ComponentB</h3>
  <p>{{str}}</p>
  <p v-for="(str,index) of arr_test" :key="index">{{str}}</p>
</template>

<script>
//1. 数字和字符串可以直接default,但是如果是数组或者对象，必须通过工厂函数返回默认值
//2. 子组件无法在修改父组件传过来的数据
export default {
  data(){
    return {

    }
  },
  props:{
    str:{
      type:[String,Number],//类型现在
      required:true, // 必须性
      default: "默认的",//默认值
    },
    arr_test:{
      type: Array,
      default(){
        return ["空"]
      }

    }
  },
}
</script>

<style scoped>

</style>