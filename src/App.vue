<template>
  <div class="background">
    <div class="wrapper">
          <Navbar></Navbar>
          <Main></Main>
    </div>
  </div>
</template>


<script>
import Navbar from "@/components/NavBar.vue";
import Main from '@/components/Main.vue'
export default {
  components: {
    Navbar,
    Main
  }
}
</script>


<style>
.wrapper{
  max-width: 1180px;
  margin: 0 auto;
  padding-top: 28px;
}

.background{
  background: var(--Linear, linear-gradient(103deg, #FCEED5 6.43%, #FCEED5 78.33%, #FFE7BA 104.24%));
}
</style>
