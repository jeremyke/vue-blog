<template>
  <div class="common-layout">
    <el-container>
      <el-aside width="25%"><Aside/></el-aside>
      <el-container>
        <el-header><Header/></el-header>
        <el-main><Main/></el-main>
        <el-footer><Footer/></el-footer>
      </el-container>
    </el-container>
  </div>
</template>

<script>

import {defineComponent} from "vue";
import Header from "@/components/Header.vue";
import Aside from "@/components/Aside.vue";
import Main from "@/components/Main.vue";
import Footer from "@/components/Footer.vue";

export default defineComponent({
  components: {Footer, Main, Aside, Header}
})
</script>

<style scoped>

</style>
