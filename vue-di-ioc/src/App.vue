<template>
  <h3>APP根组件</h3>
  <Parent :title="msg"/>
</template>

<script>


import Parent from "@/components/Parent.vue";

export default {
  name: "App",
  components: {Parent},
  data(){
    return{
      msg:"xxxx",
      content:"APP的内容"
    }
  },
  methods:{

  },
  provide(){
    return{
      showMsg:"app的数据",
      content:this.content,
    }
  },

}
</script>

<style scoped>

</style>