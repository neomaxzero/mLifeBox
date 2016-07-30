
<template>
  <modal :show.sync="show">
       <h3 slot="header">Configuration</h3>

  </modal>
</template>

<script>
import modal from '../components/modal/modal'


export default {
  components:{
    modal
  },
  props: {
    show: {
      type: Boolean,
      required: true,
      twoWay: true
    }
  },
  data () {
    return {
  
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
