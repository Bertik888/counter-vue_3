<template>  
  <div class="ui-counter-block__add">
    <button class="btn">
      <div class="plus_one"></div>
      <div class="plus_two"></div>
      
      
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
    margin-left: auto;
    margin-right: auto;
    margin-top: 50px;
    height: 60px;
    width: 3px; 

  }

}


  .plus_one, 
.plus_two {
  
  margin-right: 10px;
}

.plus_one:before, 
.plus_two:before {
  content: "+";
  display: flex; 
  flex-direction: row; 
  align-items: center; 
  justify-content: center;
  height: 20px; 
  width: 3px;
  font-size: 80px; 
  line-height: 105px; 
  text-align: center; 
  color: white;
}

.plus_one::before {font-family: sans-serif; font-weight: bold;}
.plus_two::before {font-family: serif; font-weight: normal;} 


</style>