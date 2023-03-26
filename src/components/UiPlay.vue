<template>
  <div class="ui-counter-block__play">
    <button class="btn">
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