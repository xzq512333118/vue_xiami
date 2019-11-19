<template>
  <div id="app">
    
    <router-view/>
    
  </div>
</template>
<script>
  
  
  export default {
  
}
</script>
<style lang="less">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

/*  css reset*/
* {
  margin: 0;
  padding: 0; }

body{
    background-color: #eeeeee;
}
.container{
    background-color: #fff;
    width: 1300px;
}
.font_small {
    font-size: 0.8rem; }
a{
    text-decoration: none;
}

</style>
