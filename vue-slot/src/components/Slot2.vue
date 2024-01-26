<template>
  <h3>slot续集</h3>
  <slot>插槽默认值</slot>
  <hr>
  <slot name="header"></slot>
  <hr>
  <slot name="content"></slot>

</template>


<script>
export default {
  name: "Slot2"
}
</script>

<style scoped>

</style>