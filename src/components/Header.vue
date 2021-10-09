<template>
  <div id="app">
    <div id="nav">
      <h3>San <em>Parrilla</em></h3>
      <router-link to="/">Inicio</router-link>
      <router-link to="/about">Productos</router-link>
      <router-link to="/contact">Contáctanos</router-link>
      <router-link to="/Nota">Pedido</router-link>
    </div>
    <router-view/>
  </div>
  
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  background: #333;
  text-align: center;

  
  a {
    font-weight: bold;
    color: white;
    padding: 15px;
    font-size: 20px;
    text-decoration: none;
    margin-right: 5px;

    &.router-link-exact-active {
      color: #f33f3f;
      
    }
  }
  a:hover{
    background: #ddd;
    color: #333;
  }
  h3{
    em{
      color: #f33f3f;
    }
    font-family: 'Times New Roman', Times, serif;
    float: left;
    color: white;
    text-align: center;
    padding-left: 5%;
  }
}
</style>