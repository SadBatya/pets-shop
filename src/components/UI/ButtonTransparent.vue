<template>
  <button class="button">
    {{ title }}
    <i></i>
  </button>
</template>
<script>
export default {
  name: 'button-transparent',
  props: {
    title: String,
  },
};
</script>
<style scoped>
button {
  display: flex;
  align-items: center;
  padding: 14px 28px 10px 28px;
  justify-content: center;
  border-radius: 57px;
  border: 1.5px solid var(--primary-color-dark-blue, #003459);
  gap: 8px;
  color: var(--primary-color-dark-blue, #003459);
}
i{
  display: block;
  content: '';
  background: url(./../../assets/icons/playIcon.png);
  width: 24px;
  height: 24px;
}
</style>
