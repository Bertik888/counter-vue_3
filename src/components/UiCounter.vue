<template>
    <div>  
      <p>Выключеный счётчик</p> 
    </div>

    <div class="ui-counter-block">
      <div class="ui-counter-block__time">
        <ui-timer 
          
          class="my-timer"

          
        />

      </div>

      <div class="ui-counter-block__item">

        <ui-play 
          class="my-play"
          v-model="form.name.value"
        />

        <ui-stop
          class="my-stop"
        />

      </div>

    </div>

    <div>  
      <p>Включеный счётчик</p> 
    </div>

    <div class="ui-counter-block">   

      <div class="ui-counter-block__time">
        1:20:36
      </div>

      <div class="ui-counter-block__item">

        <ui-pause
          class="my-pause"
        />

        <ui-stop
          class="my-stop"
        />
      </div>   

    </div>   

    <div class="ui-counter-block">
      <div class="ui-counter-block__item">

        <ui-add-button 
        class="my-add"/>

      </div>
    </div>

</template>

<script>
import UiPlay from '@/components/UiPlay.vue'
import UiStop from '@/components/UiStop.vue'
import UiPause from '@/components/UiPause.vue'
import UiAddButton from '@/components/UiAddButton.vue'
import UiTimer from '@/components/UiTimer.vue'

  export default {
    name: 'UiCounter',

    components: {
      UiPlay,
      UiStop,
      UiPause,
      UiAddButton,
      UiTimer
    },
    
    data() {
      return {
        form: {
          name: {
            value: '',
          }
        }
      }
    }
  }
</script>

<style lang="scss" scoped>
$font-family: 'Gotham Pro', sans-serif;
$text-color: #9E9E9E;

$control-color: #FFFFFF;
$counter-color-bg: #696969;

$counter-border: 1px solid #9E9E9E;

// $btn: border: none;
// $btn: outline: none;  // как правильно написать ? 
// $btn: background: none;

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
    flex-shrink: 0;

  }
}

</style>

