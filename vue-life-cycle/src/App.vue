<template>
<!--  <UseComponent></UseComponent>-->
  <keep-alive>
    <Component :is="tabComponent"></Component>
  </keep-alive>
  <button @click="changeCP">切换组件</button>
</template>

<script>
import UseComponent from "@/components/UseComponent.vue";
import ComponentA from "@/components/ComponentA.vue";
//import ComponentB from "@/components/ComponentB.vue";
import {defineAsyncComponent} from "vue";
const ComponentB = defineAsyncComponent(() =>
  //异步加载组件
  import("./components/ComponentB.vue")
);

export default {
  name: "App",
  components: {ComponentB, ComponentA, UseComponent},
  data(){
    return{
      tabComponent:"ComponentA"
    }
  },
  methods:{
    changeCP(){
      if(this.tabComponent === "ComponentA") {
        this.tabComponent = "componentB"
      }else{
        this.tabComponent = "ComponentA"
      }
    }
  }
}
</script>

<style scoped>

</style>