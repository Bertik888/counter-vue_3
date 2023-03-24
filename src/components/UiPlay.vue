<template>
    <div class="ui-counter-block">
      <div class="ui-counter-block__time">
        1:20:35
      </div>

      <div class="ui-counter-block__item">

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
      </div>
    </div>
</template>

<script>
  export default {
    name: 'UiPlay',
    
  }
</script>

<style lang="scss" scoped>

.btn {
  border: none;
  outline: none;
}

.ui-counter-block {
  width: 225px;
  height: 120px;
  left: 762px;
  margin-top: 72px;

  &__time {

    font-style: normal;
    font-weight: 400;
    font-size: 22px;
    line-height: 21px;
    text-align: center;
    padding: 20px 75px 20px;  // hz hz hz hz h zhz hzh zh hz 
    
    margin-bottom: 20px;
  }

  &__item {
    display: flex;
    justify-content: space-evenly;

  }
}

</style>