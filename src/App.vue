<template>
  <div id="App">
    <div class = "bg-[#F5F5F5]">
      <Header></Header>
    </div>
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  export default{
    name: "app",
    components:{
      Header,
    },  
  }
</script>