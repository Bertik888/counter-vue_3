<template>
    <div>  
      <p>Выключеный счётчик</p> 
    </div>

    <div class="ui-counter-block">
      <div class="ui-counter-block__time">
        1:20:35
      </div>

      <div class="ui-counter-block__item">

        <div class="ui-counter-block__play">
          <svg 
            width="17" 
            height="20" 
            viewBox="0 0 17 20" 
            fill="none" 
            xmlns="http://www.w3.org/2000/svg"
          >
            <path 
              d="M0 20V0L17 10L0 20Z" 
              fill="#9E9E9E"
            />
          </svg>  
        </div>      
      

        <div class="ui-counter-block__stop">
          <svg 
            width="20" 
            height="20" 
            viewBox="0 0 20 20" 
            fill="none" 
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect 
              width="20" 
              height="20" 
              fill="#9E9E9E"
            />
          </svg>
        </div>

      </div><!-- //ui-counter-block__item -->      
    </div>

    <div>  
      <p>Включеный счётчик</p> 
    </div>

    <div class="ui-counter-block">
      <div class="ui-counter-block__time">
        1:20:36
      </div>

      <div class="ui-counter-block__item">

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
      

        <div class="ui-counter-block__stop">
          <svg 
            width="20" 
            height="20" 
            viewBox="0 0 20 20" 
            fill="none" 
            xmlns="http://www.w3.org/2000/svg"
          >
            <rect 
              width="20" 
              height="20" 
              fill="#9E9E9E"
            />
          </svg>
        </div>

      </div><!-- //ui-counter-block__item -->      
    </div>

</template>

<script>
  export default {
    
  }
</script>

<style lang="scss" scoped>
$font-family: 'Gotham Pro', sans-serif;
$text-color: #9E9E9E;

$control-color: #FFFFFF;
$counter-color-bg: #696969;

$counter-border: 1px solid #9E9E9E;

.ui-counter-block {
  width: 225px;
  height: 120px;
  left: 762px;
  margin-top: 72px;
  color: $text-color;
  background: $counter-color-bg;
  font-family: $font-family;

  &__time {

    font-style: normal;
    font-weight: 400;
    font-size: 22px;
    line-height: 21px;
    text-align: center;
    padding: 20px 75px 20px;  // hz hz hz hz h zhz hzh zh hz 
    border-bottom: $counter-border;
    margin-bottom: 20px;
  }

  &__item {
    display: flex;
    justify-content: space-evenly;

  }

  &__pause {
    // display: flex;
    // justify-content: space-between;

    position: relative;    
    width: 3px;
    height: 20px;
    background: $control-color;
  }

  &__pause_left {

  }

  &__pause_right {
    position: absolute;
  width: 3px;
  height: 20px;
  top: 0;
  right: 0;
    
  }
}

</style>

