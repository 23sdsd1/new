<template>
  
 <div>
     <my-header></my-header>
   

 </div>


</template>



<script>
import myHeader from '../components/myHeader'
export default {
  head: {
    title: "简书-创作你得创作",                                                                                                                
    meta: [
      { charset: "utf-8" },
      { name: "keyword", content: "简书首页" },
      { name: "description", content: "简书" },
      { name: "author", content: "沈龙" }
    ]
  },
  components:{
      myHeader
  },
  data() {
    return {
      name: "首页"
    };
  }
};
</script>


<style>


</style>

