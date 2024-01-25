<template>
  <h3>Child</h3>
  <p>{{title}}</p>
  <p>{{demo}}</p>
</template>

<script>
export default {
  data(){
    return {

    }
  },
  props:["title","demo"],
}
</script>

<style scoped>

</style>