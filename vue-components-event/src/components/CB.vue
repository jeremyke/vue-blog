<template>
  <h3>CB</h3>
  <p>{{title}}</p>
  <p>{{onEvent("传递数据")}}</p>
</template>

<script>
export default {
  name: "CB",
  props:{
    title:String,
    onEvent: Function
  },
  methods:{
  }
}
</script>

<style scoped>

</style>