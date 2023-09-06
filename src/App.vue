<template>
  <div class="wrapper">
      <nav>
        <navbar></navbar>
      </nav>
  </div>
</template>


<script>
import Navbar from "@/components/NavBar.vue";

export default {
  components: {
    Navbar
  }
}
</script>


<style>
.wrapper{
  max-width: 1180px;
  margin: 0 auto;
  padding-top: 28px;
  padding-bottom: 28px;
  
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}



nav a {
  font-weight: bold;
  color: #2c3e50;
}

</style>
