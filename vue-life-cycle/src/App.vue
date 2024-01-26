<template>
<!--  <UseComponent></UseComponent>-->
  <Component :is="tabComponent"></Component>
  <button @click="changeCP">切换组件</button>
</template>

<script>
import UseComponent from "@/components/UseComponent.vue";
import ComponentA from "@/components/ComponentA.vue";
import ComponentB from "@/components/ComponentB.vue";
import componentB from "@/components/ComponentB.vue";

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