<template>
  <div class="box" @click="show" v-bind:class="{'boxFilled':passed}">

  </div>
</template>

<script>
export default {
  props:['val','index','avgYears'],
  methods:{
    show:function(){
      console.log('Pressed'+ this.index);
    }
  },
  computed:{
    passed:function(){
       var birthday = new Date(1990,4,11);
       var now = new Date();
       var diff = now - birthday;
       var actualWeek = diff/1000/60/60/24/7;
       var iWeek = parseInt(actualWeek);
       return  this.index<iWeek-1;
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
  h1 {
    color: #888;
  }

  .box{
      border-radius: 3px;
      border: 1px solid #AAA;
      margin: 1px;
      height: 10px;
      width: 10px;
  }

  .boxFilled{
      border-radius: 3px;
      border: 1px solid #AAA;
      background-color: #EEE;
      margin: 1px;
      height: 10px;
      width: 10px;
  }
  .box:hover{
    border: 1px solid #100;
  }
</style>
