<template>
  <h3>计算属性</h3>
  <p>{{objValMsg}}</p>
  <ul v-for="(name,index) of nameArr">
    <li :key="index">{{name}}</li>
  </ul>
</template>

<script>
export default {
  //属性
  data(){
    return {
      objVal:{
        msg:"hello",
        nameArr:["abc","def","ghi"],
      }
    }
  },
  //计算属性
  computed:{
    objValMsg(){
      return this.objVal.msg.length>0?"yes":"no"
    }
  },
  //方法
  methods:{

  }
}
</script>