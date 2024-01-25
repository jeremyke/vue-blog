<template>
<h3>Parent</h3>
  <Child :title="msg" demo="测试"/>
</template>

<script>

import Child from "@/components/Child.vue";

export default {
  components: {Child},
  data(){
    return {
      msg:"parent-msg",
    }
  }
}
</script>

<style scoped>

</style>