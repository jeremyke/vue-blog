<template>
  <h3>ComponentA</h3>
  <p>{{msg}}</p>
  <button @click="changeHandle">更新数据</button>
</template>

<script>
export default {
  name: "ComponentA",
  beforeUnmount() {
    console.log("beforeUnmount")
  },
  unmounted() {
    console.log("unmounted")
  },
  data(){
    return{
      msg:"老数据"
    }
  },
  methods:{
    changeHandle(){
      this.msg = "新数据"
    }
  }
}
</script>

<style scoped>

</style>