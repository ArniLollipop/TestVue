<template>
  <div class = "container mx-auto px-5 py-4 mt-2">
    <div class = "w-full" v-for="list in list_class" v-bind:key="list.text_class">
      <div class = "w-full h-[50%] border-b border-gray relative mt-4 pb-2">
        <div class = "">
          <div :class="list.bg_class">
          </div>
        </div>
        <div class = "grid grid-cols-11 ml-4">
          <div class = "w-full col-span-6">
            <span class = "font-bold text-xs text-[#686D7B]">Text</span>
          </div>
          <div class = "w-full col-span-2">
            <span class = "font-bold text-xs text-[#686D7B]">Text</span>
          </div>
          <div class = "w-full col-span-1">
            <span class = "font-bold text-xs text-[#686D7B]">Text</span>
          </div>
          <div class = "w-full col-span-1">
            <span class = "font-bold text-xs text-[#686D7B]">Итого, $</span>
          </div>
        </div>
        <div class = "grid grid-cols-11 ml-4">
          <div class = "w-full col-span-6">
            <span :class="list.text_class">#23</span>
            <span class = "ml-4">Text</span>
          </div>
          <div class = "w-full col-span-2">
            <span :class="list.text_class">Text</span>
          </div>
          <div class = "w-full col-span-1 font-semibold">
            <span>00:</span>
            <span :class="list.text_class">12:34</span>
          </div>
          <div class = "w-full col-span-1">
            <span class = "font-semibold text-sm">2 340,0</span>
          </div>
        </div>
        <div class = "grid grid-cols-11 mt-2 items-center ml-4">
          <div class = "w-full col-span-6">
            <span class = "text-sm text-[#686D7B]">Text</span>
          </div>
          <div class = "w-full cols-span-5">
            <div class = "w-full flex items-center gap-x-2">
              <div class = "bg-[#EBF2FF] rounded-md w-full col-span-1 flex items-center gap-x-2 px-2 py-1">
                <div class = "h-2 w-2 bg-[#FFC805] rounded-full">

                </div>
                Metka
              </div>
              <div class = "bg-[#EBF2FF] rounded-md w-full col-span-1 flex items-center gap-x-2 px-2 py-1">
                <div class = "h-2 w-2 bg-[#FFC805] rounded-full">

                </div>
                Metka
              </div>
              <div class = "bg-[#EBF2FF] rounded-md w-full col-span-1 flex items-center gap-x-2 px-2 py-1">
                <div class = "h-2 w-2 bg-[#FFC805] rounded-full">

                </div>
                Metka
              </div>
              <div class = "bg-[#EBF2FF] rounded-md w-full col-span-1 flex items-center gap-x-2 px-2 py-1">
                <div class = "h-2 w-2 bg-[#FFC805] rounded-full">

                </div>
                Metka
              </div>
            </div>
          </div>
        </div>
        <div class = "grid grid-cols-6 mt-4 gap-x-4 ml-4">
          <div class = "col-span-1 w-full ">
            <span class = "text-sm text-[#828282] ">Имя</span>
          </div>
          <div class = "col-span-1 w-full ">
            <span class = "text-sm text-[#828282] ">Text</span>
          </div>
          <div class = "col-span-1 w-full ">
            <span class = "text-sm text-[#828282] ">Text</span>
          </div>
          <div class = "col-span-1 w-full ">
            <span class = "text-sm text-[#828282] ">Status:Text</span>
          </div>
          <div class = "col-span-1 w-full ">
            <span class = "text-sm text-[#828282] ">Text</span>
          </div>
          <div class = "col-span-1 w-full ">
            <span class = "text-sm text-[#828282] ">Имя</span>
          </div>
        </div>
        <div class = "absolute top-2 right-2 flex items-center gap-x-5">
          <Stop/>
          <Dots/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import Stop from '@/icons/Stop.vue';
  import Dots from '@/icons/Dots.vue';
  export default{
    name:"App-List",
    props:{
      list_class:{},
    },
    components:{
      Stop,
      Dots,
    }
  }
</script>