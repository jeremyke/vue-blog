<template>
  <h3>Child</h3>
  <button @click="clickEventHandle">传递数据</button>
</template>

<script>
export default {
  name: "Child",
  methods:{
    clickEventHandle(){
      console.log("child button")
      this.$emit("someEvent","child数据")
    }
  }
}
</script>

<style scoped>

</style>