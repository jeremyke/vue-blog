<template>
<h3>Parent</h3>
  <Child :title="msg" demo="测试" :age="age" :arr_test="arr_test" :people="people"/>
</template>

<script>

import Child from "@/components/Child.vue";

export default {
  components: {Child},
  data(){
    return {
      msg:"parent-msg",
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