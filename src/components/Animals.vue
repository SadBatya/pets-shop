<template>
  <div class="animals">
    <div class="text">
      <h4>Whats new?</h4>
      <h2>Take a look at some of our pets</h2>
    </div>
    <ButtonArrow title="View more"></ButtonArrow>
  </div>
  
</template>
<script>
import ButtonArrow from './UI/ButtonArrow.vue';
export default {
  components:{
    ButtonArrow
  }
};
</script>
<style scoped>

.animals{
  display: flex;
  justify-content: space-between;
  align-items: flex-end;
  padding-top: 60px;
}

h4 {
  color: #000;
  font-size: 16px;
  font-weight: 500;
  line-height: 24px;
}
h2 {
  color: var(--primary-color-dark-blue, #003459);
  font-family: SVN-Gilroy;
  font-size: 24px;
  font-weight: 700;
  line-height: 36px;
  text-transform: capitalize;
}
</style>
