<template>
  <div class = "mx-auto px-5 container mt-5">
    <div class = "grid grid-cols-6 gap-x-5">
      <div v-for="classes in text_class" v-bind:key="classes.class" class = "col-span-1">
        <button :class="classes.class">
          <p>Text</p>
          <ChevronDown/>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
  import ChevronDown from '@/icons/ChevronDown.vue';
  export default{
    name : "Filter_Text",
    props:{
      text_class:{},
    },
    components:{
      ChevronDown,
    }
  }
</script>