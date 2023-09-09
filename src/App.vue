<template>
  <div class="background">
    <div class="wrapper">
      <Navbar></Navbar>
      <Main></Main>
    </div>
  </div>
  <div class="wrapper">
    <Animals></Animals>
  </div>
</template>

<script>
import Animals from './components/Animals.vue';
import Navbar from '@/components/NavBar.vue';
import Main from '@/components/Main.vue';
export default {
  components: {
    Navbar,
    Main,
    Animals,
  },
};
</script>

<style>


.wrapper {
  max-width: 1180px;
  margin: 0 auto;
  padding-top: 28px;
}

.background {
  background: var(
    --Linear,
    linear-gradient(103deg, #fceed5 6.43%, #fceed5 78.33%, #ffe7ba 104.24%)
  );
}
</style>
