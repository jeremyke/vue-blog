<template>
  <h3>文本插值</h3>

  <p>打招呼: {{ name }}</p>
</template>

<script>
export default {
  data() {
    return{
      name: "你好呀👋"
    }
  }
}
</script>