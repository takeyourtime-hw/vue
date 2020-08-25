<template>
  <div class="about">
    <h1>This is an about page</h1>
    <h1>{{msg}}</h1>
  </div>
</template>
<script>
export default {
  data(){
    return{
      msg:"法撒结局司法局哦i哇"
    }
  },
  created(){
    this.$http.get("/api/w/website/bannerList").then(res=>{
      console.log(res)
    })
  }
}
</script>
