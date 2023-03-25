<template>
  <div class="ui-counter-block__pause">

    <div class="ui-counter-block__pause_left">
      <svg 
        width="3" 
        height="20" 
        viewBox="0 0 3 20" 
        fill="none" 
        xmlns="http://www.w3.org/2000/svg"
      >
        <rect width="3" height="20" fill="white"/>
      </svg>
    </div>

    <div class="ui-counter-block__pause_right">
      <svg 
        width="3" 
        height="20" 
        viewBox="0 0 3 20" 
        fill="none" 
        xmlns="http://www.w3.org/2000/svg"
      >
        <rect width="3" height="20" fill="white"/>
      </svg>
    </div>

  </div>  
</template>

<script>
  export default {
    name: 'UiPause'
    
  }
</script>

<style lang="scss" scoped>

.ui-counter-block {
  &__pause {
    position: relative; 
    height: 20px;
    background: #FFFFFF;
  }
    &__pause_left {
      position: absolute;
    }

    &__pause_right {
      position: absolute;
      padding-left: 5px;      
    }
}

  

</style>