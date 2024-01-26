<template>
  <Base>
    <div>
      <h3>插槽标题</h3>
      <p>插槽内容</p>
    </div>
  </Base>
  <p>-----------</p>
  <Slot2>
    <template #header>
      <p>{{headerMsg}}</p>
    </template>
    <template v-slot:content>
      <p>{{contentMsg}}</p>
    </template>
  </Slot2>
  <p>-----------</p>
  <Slot3>
    <template #abc="slotProps">
      <h3>{{slot3_data.currentTest}}---{{slotProps.msg}}</h3>
    </template>
    <template #efg="slotProps">
      <h3>{{slot3_data.msg}}---{{slotProps.msg}}</h3>
    </template>
  </Slot3>

</template>

<script>
import Base from "@/components/Base.vue";
import Slot2 from "@/components/Slot2.vue";
import Slot3 from "@/components/Slot3.vue";

export default {
  components:{
    Slot3,
    Slot2,
    Base
  },
  data(){
    return{
      msg:"插槽内容续集aa",
      headerMsg:"插槽标题啊啊啊",
      contentMsg:"插槽内容啊啊啊",
      slot3_data:{
        msg:"插槽内容再续集",
        currentTest:"测试内容",
      },
    }
  }
}
</script>

<style scoped>
</style>
