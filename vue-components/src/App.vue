<template>
  <!-- 3.显示组件 -->
  <MyComponent  />

  <my-component  />
</template>

<script>
//1. 引入组件
import  MyComponent from "./components/MyComponent.vue"
//2. 注入组件
export default {
  components:{
    MyComponent
  }
}
</script>