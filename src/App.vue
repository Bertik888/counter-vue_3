<template>
  <div class="container">

    <div class="row">            
      
      <ui-counter 
        class="my-counter" 
      
      />
    </div>
    
  </div>

</template>

<script>
import UiCounter from './components/UiCounter.vue'


export default {
  name: 'App',
  components: {
    UiCounter
  },

  data() {

  },
}
</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&display=swap');

*, ::after, ::before {
  box-sizing: border-box;
}

#app {
  font-family: 'Gotham Pro', 'Roboto', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.container {
  width: 100%;
  max-width: 1024px;
  padding-right: 212px;
  padding-left: 212px;
  margin-right: auto;
  margin-left: auto;
}

.row { 
  // display: flex;
  flex-wrap: wrap;

}
</style>
