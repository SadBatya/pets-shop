<template>
  <div class="main">
    <div class="main__text">
      <h1>One more friend</h1>
      <h2>Thousands more fun!</h2>
      <p>
        Having a pet means you have more joy, a new friend, a happy person who
        will always be with you to have fun. We have 200+ different pets that
        can meet your needs!
      </p>

      <div class="buttons">
        <ButtonTransparent title="View Intro"></ButtonTransparent>
        <my-button class="button__blue" title="Explore Now"></my-button>
      </div>
    </div>
    <div class="main__image"></div>
  </div>
</template>
<script>
import MyButton from './UI/ButtonBlue.vue';
import ButtonTransparent from './UI/ButtonTransparent.vue';
export default {
  components: {
    MyButton,
    ButtonTransparent
  },
};
</script>
<style scoped>
.main {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.main__text{
  width: 550px;
  color: var(--primary-color-dark-blue-80, #002a48);
}

.main__image{
  content: '';
  background: url(./../assets/pets/header__dog.png);
  width: 800px;
  height: 611px;
  background-position: center;
  
}

.buttons{
  display: flex;
  height: 48px;
  gap: 20px;
}

.button__blue{
  height: 48px;
}

h1 {
  font-family: SVN-Gilroy;
  font-size: 60px;
  font-weight: 800;
  line-height: 68px;
  text-transform: capitalize;
  margin-bottom: 4px;
}

h2 {
  font-family: SVN-Gilroy;
  font-size: 46px;
  font-weight: 700;
  line-height: 60px; 
  text-transform: capitalize;
  margin-bottom: 24px;
}

p {
  text-align: left;
  font-family: SVN-Gilroy;
  font-size: 16px;
  font-weight: 500;
  line-height: 24px;
  margin-bottom: 34px;
}
</style>
