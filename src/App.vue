<template>
  <div id="App">
    <div class = "">
      <Header></Header>
      <NavbarVue></NavbarVue>
    </div>
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  import NavbarVue from './components/Navbar.vue';
  export default{
    name: "app",
    components:{
      Header,
      NavbarVue,
    },  
  }
</script>