<template>  
  <div class="ui-counter-block__add">
    <button class="btn">

      <div class="plus_one">
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

      <div class="plus_two">
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
      
      
    </button>
  </div>
</template>

<script>
  export default {
    name: 'UiAddButton'
    
  }
</script>

<style lang="scss" scoped>
.ui-counter-block {
  &__add {
    // margin-left: auto;
    // margin-right: auto;
    margin: 0 auto;
    position: relative;
  }
}
.plus_one {
  position: absolute;
  top: 50px;
}
.plus_two {
    position: absolute;
    transform: rotate(-90deg);
    top: 48px;
    left: 7px;
}
</style>