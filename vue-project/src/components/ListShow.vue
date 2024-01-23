<template>
  <h3>列表渲染</h3>
  <p v-for="val of arrTest">{{val}}</p>
  <ul v-for="meta of list">
    <li :id="meta.id">{{meta.content}}----{{meta.linkStr}}</li>
  </ul>

  <p v-for="(val,index) of arrTest">{{index}}---{{val}}</p>

  <div v-for="(value,key,index) of objVal">{{index}}--{{key}}---{{value}}</div>

</template>

<script>
  export default {
    data() {
      return {
        arrTest: ["我","你","他"],
        list:[
          {
            id:123,
            content:"dsdsvebrebfdvfdbdfbd",
            linkStr:"xxxq1",
          },
          {
            id:124,
            content:"fdvfrbtrntntny",
            linkStr:"xxxq2",
          },
          {
            id:125,
            content:"ddfbbrtbtnryddddd",
            linkStr:"xxxq3",
          }
        ],
        objVal:{
          name:"xxx",
          age:12,
          sex:"女"
        }
      }
    }
  }
</script>