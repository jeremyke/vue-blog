<template>
  <h3>属性绑定</h3>
  <div v-bind:id="idVal" v-bind:class="classVal" v-bind:title="titleVal">测试1</div>
  <div v-bind:title="titleNulVal">测试2</div>
  <div :id="idVal" :class="classVal" :title="titleVal">测试3</div>
  <button :disabled="displayVal">测试4</button>
  <div :id="objVal.idVal" :class="objVal.classVal" :title="objVal.titleVal">测试5</div>
</template>

<script>
  export default {
    data() {
      return {
        classVal: "active",
        idVal: "app123",
        titleVal: "xxx",
        titleNulVal: null,
        displayVal: true,
        objVal: {
          classVal: "active",
          idVal: "app123",
          titleVal: "xxx",
        }

      }
    }
  }
</script>