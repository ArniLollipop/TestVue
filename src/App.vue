<template>
  <div id="App">
    <Header></Header>
      <Navbar/>
      <div class = "bg-[#F5F5F5] pb-2 mt-2"> 
        <Filters class = ""></Filters>
        <Filter_Button :button_class="buttons_class"/>
      </div>
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  import Navbar from './components/Navbar.vue';
  import Filters from './components/Filters.vue';
  import Filter_Button from './components/Filter_Button.vue';
  export default{
    name: "app",
    components:{
      Header,
      Navbar,
      Filters,
      Filter_Button,
    },  
    data(){
      return{
        buttons_class:[
          {alert_class:"hidden", left_class:"w-1 z-10 h-full bg-[#F2994A]", class: "flex z-0 items-center overflow-hidden w-[57px] h-[36px] bg-[#42A5F5] rounded-md text-white"},
          {alert_class:"hidden", left_class:"w-1 z-10 h-full bg-[#08257A]", class: "flex z-0 items-center overflow-hidden w-[57px] h-[36px] bg-[#F2F2F2] rounded-md"},
          {alert_class:"", left_class:"w-1 z-10 h-full bg-[#9B51E0]", class: "flex z-0 items-center pr-2 overflow-hidden w-[89px] h-[36px] bg-[#F2F2F2] rounded-md"},
          {alert_class:"hidden", left_class:"w-1 z-10 h-full bg-[#27AE60]", class: "flex z-0 items-center overflow-hidden w-[57px] h-[36px] bg-[#F2F2F2] rounded-md"}
        ]
      }
    }
  }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700;900&display=swap');
</style>