<template>
  <h3>CA</h3>
  <CB title="标题" :onEvent="dataFn" />
  <p>{{msg}}</p>
</template>

<script>
import CB from "@/components/CB.vue";

export default {
  name: "CA",
  data(){
    return{
      msg:"",
    }
  },
  components: {CB},
  methods:{
    dataFn(data){
      console.log(data);
      this.msg = data
    }
  }
}
</script>

<style scoped>

</style>