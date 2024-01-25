<template>
  <h3>Child</h3>
  <p>{{title}}</p>
  <p>{{demo}}</p>
  <p>{{age}}</p>
  <p v-for="(str,index) of arr_test" :key="index">{{str}}</p>
  <p v-for="(key,value,index) of people" :key="index">{{key}}--{{value}}</p>
</template>

<script>
export default {
  data(){
    return {

    }
  },
  props:["title","demo","age","arr_test","people"],
}
</script>

<style scoped>

</style>