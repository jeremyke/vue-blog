<template>
  <h3>模版标签</h3>
  <p>打招呼: {{ msg }}</p>
  <p>AGE: {{ age + 1 }}</p>
  <p>{{ flag?"YES":"NO" }}</p>
  <p>打招呼反转{{ msg.split("").reverse().join("") }}</p>
  <p v-html="rawHTML"></p>

</template>

<script>
export default {
  data() {
    return{
      msg: "你好呀👋",
      age: 21,
      flag:true,
      rawHTML:"<a href='https://baidu.com'>百度</a>"
    }
  },
}
</script>