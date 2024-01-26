<template>
  <h3>插槽再续集</h3>
  <slot :msg="childMsg" name="abc"></slot>
  <slot :msg="childMsg" name="efg"></slot>
</template>

<script>
export default {
  name: "Slot3",
  data(){
    return{
      childMsg:"子组件字段",
    }
  }
}
</script>

<style scoped>

</style>