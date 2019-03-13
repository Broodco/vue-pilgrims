<template>
  <div id="app">
    <ListPage :pilgrims="pilgrims" class="leftpage"></ListPage>
    <router-view class="rightpage"/>
  </div>
</template>

<script>
import ListPage from './components/ListPage.vue'
import data from './data/pilgrims.json'

export default {
  name : "app",
  components:{
    ListPage,
  },
  data(){
    return{
      pilgrims : data
    }
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display:flex;
  justify-content: space-around;
}
.leftpage{
  width : 30%;
}
.rightpage{
  width:30%;
}
</style>
