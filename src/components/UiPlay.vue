<template>
  <div class="ui-counter-block__play">
    <button 
      :value="modelValue"
      @click.prevent="startButton"
      class="btn">

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
    </button>
  </div> 
</template>

<script>
  export default {
    name: 'UiPlay',

    methods: { 
      /* startButton() {
        clearInterval(interval)
        interval = setInterval(startTimer, 10)
        console.log(interval)
      }, */



      /* async startTimer() {
        function startTimer() {
          try{ 
            if(second < 9) {
              secondElement.innerText = "0" + second
            }
            if(second > 9) {
              secondElement.innerText = second
            }
            if(second > 59) {
              minute++
              minuteElement.innerText = "0" + minute
              second = 0
              secondElement.innerText = "0" + second
            }
          } catch (e) {
            console.error(e)
          }
        }
      } */


    },
    
  }
</script>

<style lang="scss">

.btn {
  border: none;
  outline: none;
  background: none;
  align-items: center;
  cursor: pointer;
}

</style>