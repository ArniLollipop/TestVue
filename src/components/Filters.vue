<template>
  <div class = "px-[110px] flex items-center xl:justify-center py-4 mt-2">
    <div class = "flex items-center h-[41px] gap-x-3">
      <button class = "bg-white px-2 py-2 h-full rounded-md flex items-center justify-between w-[300px]">
        <p>Text</p>
        <ChevronDown/>
      </button>
      <button class = "bg-white px-2 py-2 h-full w-[704px] text-start ml-5 rounded-md flex items-center justify-between">
        <p>Text</p>
        <Sliders/>
      </button>
      <button class = "bg-[#42A5F5] px-5 h-full rounded-md w-[112px] flex items-center justify-between ml-3">
        <PlusCircle/>
        <p class = "text-end">Text</p>
      </button>
      <button class = "py-2 px-3 bg-[#EBF2FF] rounded-md w-[32px] flex justify-center">
        <Dots/>
      </button>
    </div>
  </div>

</template>

<script>
import ChevronDown from '@/icons/ChevronDown.vue';
import Sliders from '@/icons/Sliders.vue';
import PlusCircle from '@/icons/PlusCircle.vue';
import Dots from '@/icons/Dots.vue';

export default {
  name: 'App-Filters',
  components:{
    ChevronDown,
    Sliders,
    PlusCircle,
    Dots,
  }
}

</script>