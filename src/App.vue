
<template>
  <div id="app">
    <chead></chead>
    <boxes></boxes>
    <cfooter></cfooter>
  </div>
</template>

<script>
import chead from './components/chead'
import cfooter from './components/cfooter'
import boxes from './Boxes/Boxes'

export default {
  components: {
    chead,
    cfooter,
    boxes
  }
}
</script>

<style>
html {
  height: 100%;
}

body {

  min-height: 96%;
}

#app {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  color: #2c3e50;


  font-family: Source Sans Pro, Helvetica, sans-serif;
  text-align: center;
}

#app a {
  color: #42b983;
  text-decoration: none;
}

</style>
