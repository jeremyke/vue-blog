<template>
  <h3>组件的生命周期</h3>
  <p>{{msg}}</p>
  <button @click="updateData">更新数据</button>
</template>

<script>

/*
 * 生命周期函数
 * 创建期
 * beforeCreate
 * created
 * 挂载期
 * beforeMount
 * mounted
 * 更新期
 * beforeUpdate
 * updated
 * 销毁期
 * beforeUnmount
 * unmounted
 */
export default {
  data(){
    return{
      msg:"xxx"
    }
  },
  methods:{
    updateData(){
      this.msg = "更新啦"
    }
  },
  beforeCreate(){
    console.log("beforeCreate");
  },
  created() {
    console.log("created");

  },
  beforeMount() {
    console.log("beforeMount");

  },
  mounted() {
    console.log("mounted");

  },
  beforeUpdate() {
    console.log("beforeUpdate");

  },
  updated() {
    console.log("updated");

  },
  beforeUnmount() {
    console.log("beforeUnmount");

  },
  unmounted() {
    console.log("unmounted");

  },
}
</script>

<style scoped>
</style>