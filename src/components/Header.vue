<template>
  <section class = " w-full">
    <div class = "bg-white border-b border-[#E0E3EB] w-full">
      <div class = "px-[110px] py-4 flex items-center justify-between">
        <div class = "flex items-center gap-x-5">
          <LogoMenu/>
          <p class = "text-3xl font-bold text-[#42A5F5]">LOGO</p>
        </div>
        <div class = "flex items-center">
          <button class = "pl-6 pr-3 py-2 bg-[#EBF2FF] rounded-3xl flex items-center">
            <span class = "before:bg-[#FFC805] before:h-2 before:w-2 before:rounded-full before:absolute before:top-1/2 before:-translate-y-1/2 relative before:-left-4 w-[236px] text-start">Text</span>
            <p class = "text-base font-semibold text-[#12192F] mr-2">00:<span class = "text-[#42A5F5]">05:43</span></p>
            <Stop/>
          </button>
          <div class = "ml-6 relative">
            <BellIcon :className="qwe"/>
            <span class = "text-white bg-[#FF2E53] w-4 h-4 text-center text-xs rounded-full absolute top-1/3">38</span>
          </div>
          <div class = "h-[50px] w-[50px] rounded-full overflow-hidden bg-purple-500 ml-6">
            <img src="@/img/icon-park-outline_application-menu.svg" alt="">
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import BellIcon from "../icons/BellIcon.vue";
import LogoMenu from "@/icons/LogoMenu.vue";
import Stop from "@/icons/Stop.vue";

export default {
  name: 'App-Header',
  components:{
    BellIcon,
    LogoMenu,
    Stop,
  },
  data() {
    return {
      qwe: "w-10 h-10"
    }
  }
}
</script>