<template>
  <h3>ComponentA</h3>
  <ComponentB :str="msg" :arr_test="arr_test"/>
</template>

<script>

import ComponentB from "@/components/ComponentB.vue";

export default {
  components: {ComponentB},
  data(){
    return {
      msg:"a-msg字符串",
      age: 13,
      arr_test:["aa","bb","cc"],
      people:{
        name:"xx",
        sex:"男",
        age:23,
      }
    }
  }
}
</script>

<style scoped>

</style>