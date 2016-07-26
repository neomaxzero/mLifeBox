<template>
  <div class="boxes">

      <Box v-for="1 in cant"  :index="$index" :avg-years="avgYears">
      </Box>


  </div>
</template>

<script>
import Box from './Box'

export default {
  props:{
    cant:{
      type:Number,
      default:4171
    }
  },
  components: {
    Box
  },

  data () {
    return{
      avgYears:80
    }
  }

}



var getBoxes= function(avgYears){
    return (365/7*avgYears).toFixed();

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1 {
    color: #888;
  }

  .boxes{
      display: flex;
      flex-direction: row;
      flex-wrap: wrap;
      align-content: flex-start;
      height: 80%;
  }
</style>
