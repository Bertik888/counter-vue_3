<template>
  <div class="timer">   
    {{ time }}
    
    <!-- 1:20:35  -->
  </div>
</template>

<script>
  export default {
    name: 'UiTimer',

    props: {
      time: {
        type: Number,
        default: '${hour}:${minute}:${second}'
      }
    }
    
  }
</script>

<style lang="scss" scoped>

</style>
<!-- 
<div class="timer__block">
  <div class="time hour">01</div>
  <div class="title">Hours</div>
</div>

<div class="timer__block">
  <div class="time minute">20</div>
  <div class="title">Minutes</div>
  </div>

<div class="timer__block">
  <div class="time second">35</div>
  <div class="title">Seconds</div>
</div> -->