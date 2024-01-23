<template>
  <h3>表单输入与绑定</h3>
  <input type="text" v-model="msg">
  <p>{{msg}}</p>

  <input type="checkbox" id="checkbox" v-model="checked">
  <label for="checkbox">{{checked}}</label>

</template>

<script>
export default {
  //属性
  data(){
    return {
      msg:"",
      checked:false,
    }
  },

  //计算属性
  computed:{

  },

  //方法
  methods:{
  },

  //监听
  watch:{

  }
}
</script>

<style>

</style>