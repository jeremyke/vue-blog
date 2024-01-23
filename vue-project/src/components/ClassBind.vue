<template>
  <h3>class绑定</h3>
  <p :class="{'active':isActive,'text-danger':hasError}">测试1</p>
  <p :class="classObj">测试2</p>
  <p :class="[arrActive,arrHasError]">测试3</p>
  <p :class="[classObj]">测试4</p>

</template>

<script>
export default {
  //属性
  data(){
    return {
      isActive:true,
      hasError:false,
      classObj:{
        "active":false,
        "text-danger":true,
      },
      arrActive:"active",
      arrHasError:"text-danger",
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