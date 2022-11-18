<template>
  <div id="App">
    <Header></Header>
    <Navbar />
    <div class="bg-[#F5F5F5] pb-20 mt-2 min-h-[88vh]">
      <Filters class=""></Filters>
      <Filter_Button :button_class="buttons_class" />
      <Filter_Text :text_class="text_class" />
      <Todo v-for="item in todoList" :key="item.id" :todoList="item" />
    </div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Navbar from "./components/Navbar.vue";
import Filters from "./components/Filters.vue";
import Filter_Button from "./components/Filter_Button.vue";
import Todo from "./components/Todo.vue";
import Filter_Text from "./components/Fliter_Text.vue";
export default {
  name: "app",
  components: {
    Header,
    Navbar,
    Filters,
    Filter_Button,
    Todo,
    Filter_Text,
  },
  data() {
    return {
      buttons_class: [
        {
          alert_class: "hidden",
          left_class: "w-1 z-10 h-full bg-[#F2994A]",
          class:
            "flex z-0 items-center overflow-hidden w-[57px] h-[36px] bg-[#42A5F5] rounded-md text-white",
        },
        {
          alert_class: "hidden",
          left_class: "w-1 z-10 h-full bg-[#08257A]",
          class:
            "flex z-0 items-center overflow-hidden w-[57px] h-[36px] bg-[#F2F2F2] rounded-md",
        },
        {
          alert_class: "",
          left_class: "w-1 z-10 h-full bg-[#9B51E0]",
          class:
            "flex z-0 items-center pr-2 overflow-hidden w-[89px] h-[36px] bg-[#F2F2F2] rounded-md",
        },
        {
          alert_class: "hidden",
          left_class: "w-1 z-10 h-full bg-[#27AE60]",
          class:
            "flex z-0 items-center overflow-hidden w-[57px] h-[36px] bg-[#F2F2F2] rounded-md",
        },
      ],
      text_class: [
        {
          class:
            "flex items-center justify-between pb-4 border-b border-[#42A5F5] w-full px-1",
        },
        {
          class:
            "flex items-center justify-between pb-4 border-b border-gray w-full px-1",
        },
        {
          class:
            "flex items-center justify-between pb-4 border-b border-gray w-full px-1",
        },
        {
          class:
            "flex items-center justify-between pb-4 border-b border-gray w-full px-1",
        },
        {
          class:
            "flex items-center justify-between pb-4 border-b border-gray w-full px-1",
        },
        {
          class:
            "flex items-center justify-between pb-4 border-b border-gray w-full px-1",
        },
      ],
      todoList: [
        {
          id: 1,
          isOpen: false,
          date: "Вчера",
          time: "06:12:32",
          price: "2 340,00$",
          list: [
            {
              id: 1,
              text: "text",
              difTime: "13:09:47 – 13:09:47",
              time: "00:00:00",
              price: "2 340,0",
            },
            {
              id: 2,
              text: "text2",
              difTime: "13:09:47 – 13:09:47",
              time: "00:00:00",
              price: "2 340,0",
            },
          ],
        },
        {
          id: 2,
          isOpen: false,
          date: "Позавчера",
          time: "",
          price: "",
          list: [
            {
              id: 1,
              text: "text",
              difTime: "13:09:47 – 13:09:47",
              time: "00:00:00",
              price: "2 340,0",
            },
            {
              id: 2,
              text: "text2",
              difTime: "13:09:47 – 13:09:47",
              time: "00:00:00",
              price: "2 340,0",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700;900&display=swap");
</style>
