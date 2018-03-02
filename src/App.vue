<template>
  <div id="app">
    <h1> Liste de machine à café</h1>
   <!-- <toggle-button v-model="myDataVariable"/> -->

        <p>Cocher la case pour activer la machine </p>
    <h2 v-bind:class="{ color: checked1 }"> {{machine1}} </h2>
     <input  type="checkbox" id="checkbox" v-model="checked1">
    <h2 v-bind:class="{ color: checked2 }"> {{machine2}} </h2>
    <input  type="checkbox" id="checkbox" v-model="checked2">
 


  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      machine1: 'Machine1',
      machine2:'Machine2',
      checked1:false,
      checked2:false,
      // myDataVariable : false
    }  
  }
 

}


</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

.color {
  color : green;
}

</style>
