<template>
  <div class = "px-[115px] flex items-center gap-x-2">
    <div v-for="classes in button_class" v-bind:key="classes.class" class = "">
      
      <button :class = "classes.class">
        <div :class = "classes.left_class">
        </div>
        <div class = "flex justify-center w-full">
          <p class = ""> Text </p>
        </div>
        <Alert :class = "classes.alert_class"/>
      </button>
    </div>
  </div>
  
</template>

<script>
  import Alert from '@/icons/Alert.vue';
  export default{
    name : "App-Filter_Button",
    props:{
      button_class:{}
    },
    components:{
      Alert,
    }
  }
</script>