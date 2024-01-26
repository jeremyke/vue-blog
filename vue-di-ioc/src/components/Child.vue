<template>
  <h3>Child</h3>
  <p>{{title}}</p>
  <p>{{showMsg}}</p>
  <p>{{content}}</p>
  <p>{{globalData}}</p>
</template>

<script>
export default {
  name: "Child",
  props:{
    title:{
      type:String,
      default() {
        return "空";
      }
    }
  },
  inject:["showMsg","content","globalData"]
}
</script>

<style scoped>

</style>