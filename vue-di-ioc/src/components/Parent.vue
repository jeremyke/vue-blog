<template>
  <h3>Parent</h3>
  <Child :title="$props.title"/>
</template>

<script>
import Child from "@/components/Child.vue";

export default {
  name: "Parent",
  components: {Child},
  props:{
    title:{
      type:String
    }
  }
}
</script>

<style scoped>

</style>