<template>
  <div class="chead">
    <i class="config fa fa-cog fa-lg" aria-hidden="true"></i>
    <h1>{{ msg }}</h1>
    <div class="">

    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      // note: changing this line won't causes changes
      // with hot-reload because the reloaded component
      // preserves its current state and we are modifying
      // its initial state.
      msg: 'LifeBox'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.config{
  color: #EEE;
}

.config:hover{
  color: #CCC;
}

.chead{
  display: flex;
  justify-content: space-around;
  align-items: center;
  color: #888;
}

</style>
