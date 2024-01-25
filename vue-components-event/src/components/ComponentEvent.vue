<template>
  <h3>组件事件</h3>
  <Child @someEvent="getHandle"/>
  <p>{{msg}}</p>
</template>

<script>
import Child from "@/components/Child.vue";

export default {
  name: "ComponentEvent",
  data(){
    return{
      msg:"",
    }
  },
  components: {Child},
  methods:{
    getHandle(data){
      console.log("触发了",data);
      this.msg = data;
    }
  }
}
</script>

<style scoped>

</style>