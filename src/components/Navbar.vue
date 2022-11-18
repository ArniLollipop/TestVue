<template>
  <div class = "mt-4 bg-white">
    <div class = "container mx-auto px-5 flex items-center justify-between w-full">
      <div class = " flex items-center gap-x-4 text-sm">
        <div>
          <input type="radio" id="text1" name="text" class = "w-0 peer" checked>
          <label for="text1" class = "pb-2 peer-checked:border-b-2 cursor-pointer peer-checked:border-[#2991F5] transition-all duration-300">Text</label>
        </div>
        <div>
          <input type="radio" id="text2" name="text" class = "w-0 peer" >
          <label for="text2" class = "pb-2 peer-checked:border-b-2 cursor-pointer peer-checked:border-[#2991F5] transition-all duration-300">Text</label>
        </div>
        <div>
          <input type="radio" id="text3" name="text" class = "w-0 peer" >
          <label for="text3" class = "pb-2 peer-checked:border-b-2 cursor-pointer peer-checked:border-[#2991F5] transition-all duration-300">Text</label>
        </div>
        <div>
          <input type="radio" id="text4" name="text" class = "w-0 peer">
          <label for="text4" class = "pb-2 peer-checked:border-b-2 cursor-pointer peer-checked:border-[#2991F5] transition-all duration-300">Text</label>
        </div>
      </div>
      <button class = "flex items-center gap-x-3">
        <ChevronLeft/>
        <span class = "text-sm">Text</span>
      </button>
    </div>
  </div>
  <div class = "">

  </div>
</template>


<script>
import ChevronLeft from '@/icons/ChevronLeft.vue';
export default {
  name: 'App-Navbar',
  components:{
    ChevronLeft,
  }
}

</script>