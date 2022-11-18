<template>
  <svg :class="className" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M24 10.6666C24 8.54489 23.1571 6.51006 21.6569 5.00977C20.1566 3.50948 18.1217 2.66663 16 2.66663C13.8783 2.66663 11.8434 3.50948 10.3431 5.00977C8.84286 6.51006 8 8.54489 8 10.6666C8 20 4 22.6666 4 22.6666H28C28 22.6666 24 20 24 10.6666Z" stroke="#A9B0C2" stroke-linecap="round" stroke-linejoin="round"/>
    <path d="M18.3065 28C18.0721 28.4041 17.7356 28.7395 17.3308 28.9727C16.926 29.2059 16.467 29.3286 15.9998 29.3286C15.5327 29.3286 15.0737 29.2059 14.6689 28.9727C14.2641 28.7395 13.9276 28.4041 13.6932 28" stroke="#A9B0C2" stroke-linecap="round" stroke-linejoin="round"/>
  </svg>

</template>

<script>
  export default{
    name:'BellIcon',
    props: {
      className: {}
    },

  }
</script>