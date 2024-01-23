<template>
  <h3>条件渲染</h3>
  <div v-if="flag">true文本</div>
  <div v-else>false文本</div>

  <div v-if="type === 'A'">A</div>
  <div v-else-if="type == 'B'">B</div>
  <div v-else>C</div>

  <div v-show="showFlag">show value</div>

</template>

<script>
  export default {
    data() {
      return {
        flag: false,
        type:"D",
        showFlag: false
      }
    }
  }
</script>