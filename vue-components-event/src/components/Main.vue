<template>
  <h3>Main</h3>
  <p>{{search}}</p>
  <SearchComponent @searchEvent="getSearch"/>
</template>

<script>
import SearchComponent from "@/components/SearchComponent.vue";

export default {
  name: "Main",
  components: {SearchComponent},
  data(){
    return{
      search:""
    }
  },
  methods:{
    getSearch(data){
      this.search = data;
    }
  }
}
</script>

<style scoped>

</style>