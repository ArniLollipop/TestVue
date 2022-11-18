<template>
  <div class = "px-[100px] mt-4 bg-white">
    <div class = "flex items-center justify-between">
      <div class = " flex items-center gap-x-4 text-sm">
        <div>
          <input type="radio" id="text1" name="text" class = "w-0 peer" checked>
          <label for="text1" class = "pb-3 peer-checked:border-b-2 cursor-pointer peer-checked:border-[#2991F5] transition-all duration-300">Text</label>
        </div>
        <div>
          <input type="radio" id="text2" name="text" class = "w-0 peer" >
          <label for="text2" class = "pb-3 peer-checked:border-b-2 cursor-pointer peer-checked:border-[#2991F5] transition-all duration-300">Text</label>
        </div>
        <div>
          <input type="radio" id="text3" name="text" class = "w-0 peer" >
          <label for="text3" class = "pb-3 peer-checked:border-b-2 cursor-pointer peer-checked:border-[#2991F5] transition-all duration-300">Text</label>
        </div>
        <div>
          <input type="radio" id="text4" name="text" class = "w-0 peer">
          <label for="text4" class = "pb-3 peer-checked:border-b-2 cursor-pointer peer-checked:border-[#2991F5] transition-all duration-300">Text</label>
        </div>
      </div>
      <button class = "flex items-center gap-x-3">
        <svg width="7" height="11" viewBox="0 0 7 11" fill="none" xmlns="http://www.w3.org/2000/svg" class="mt-1">
          <path d="M6 10.5L1 5.5L6 0.5" stroke="#686D7B" stroke-linecap="round"/>
        </svg>
        <span class = "text-sm">Text</span>
      </button>
    </div>
  </div>
  <div class = "">

  </div>
</template>