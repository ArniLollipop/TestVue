<template>
  <div id="App">
    <Header></Header>
      <Navbar/>
      <div class = "bg-[#F5F5F5] pb-2 mt-2 min-h-[88vh]"> 
        <Filters class = ""></Filters>
        <Filter_Button :button_class="buttons_class"/>
        <Filter_Text :text_class="text_class"/>
        <List :list_class="list_class"/>
      </div>
  </div>
</template>

<script>
  import Header from './components/Header.vue'
  import Navbar from './components/Navbar.vue';
  import Filters from './components/Filters.vue';
  import Filter_Button from './components/Filter_Button.vue';
  import Filter_Text from './components/Fliter_Text.vue';
  import List from './components/List.vue';

  export default{
    name: "app",
    components:{
      Header,
      Navbar,
      Filters,
      Filter_Button,
      Filter_Text,
      List,
    },  
    data(){
      return{
        buttons_class:[
          {div_class:"col-span-2", alert_class:"hidden", left_class:"w-1 z-10 h-full bg-[#F2994A]", class: "flex z-0 w-full items-center overflow-hidden h-[36px] bg-[#42A5F5] rounded-md text-white"},
          {div_class:"col-span-2", alert_class:"hidden", left_class:"w-1 z-10 h-full bg-[#08257A]", class: "flex z-0 w-full items-center overflow-hidden h-[36px] bg-[#F2F2F2] rounded-md"},
          {div_class:"col-span-3", alert_class:"", left_class:"w-1 z-10 h-full bg-[#9B51E0]", class: "flex z-0 w-full items-center pr-1 overflow-hidden h-[36px] bg-[#F2F2F2] rounded-md"},
          {div_class:"col-span-2", alert_class:"hidden", left_class:"w-1 z-10 h-full bg-[#27AE60]", class: "flex z-0 w-full items-center overflow-hidden h-[36px] bg-[#F2F2F2] rounded-md"}
        ],
        text_class:[
          {class: "flex items-center justify-between pb-4 border-b border-[#42A5F5] w-full px-1"},
          {class: "flex items-center justify-between pb-4 border-b border-gray w-full px-1"},
          {class: "flex items-center justify-between pb-4 border-b border-gray w-full px-1"},
          {class: "flex items-center justify-between pb-4 border-b border-gray w-full px-1"},
          {class: "flex items-center justify-between pb-4 border-b border-gray w-full px-1"},
          {class: "flex items-center justify-between pb-4 border-b border-gray w-full px-1"},
        ],
        list_class:[
          {text_class:"text-[#42A5F5]", bg_class: "bg-[#42A5F5] w-1 h-[80%] absolute top-1/2 -translate-y-1/2 rounded-r-full"},
          {text_class:"text-[#FF2E53]", bg_class: "bg-[#FF2E53] w-1 h-[80%] absolute top-1/2 -translate-y-1/2 rounded-r-full"},
          {text_class:"text-[#219653]", bg_class: "bg-[#219653] w-1 h-[80%] absolute top-1/2 -translate-y-1/2 rounded-r-full"},
          {text_class:"text-[#42A5F5]", bg_class: "bg-[#42A5F5] w-1 h-[80%] absolute top-1/2 -translate-y-1/2 rounded-r-full"},
          {text_class:"text-[#42A5F5]", bg_class: "bg-[#9B51E0] w-1 h-[80%] absolute top-1/2 -translate-y-1/2 rounded-r-full"},
        ]
      }
    }
  }
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700;900&display=swap');
</style>