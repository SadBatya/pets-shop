<template>
  <button class="btn__blue">{{ title }}</button>
</template>
<script>
export default {
  name: 'my-button',
  props: {
    title: String
  }
}
</script>
<style scoped>
.btn__blue {
  display: flex;
  justify-content: center;
  align-items: center;
  padding-right: 28px;
  padding-left: 28px;
  font-size: 16px;
  color: #fdfdfd;
  background-color: #003459;
  height: 44px;
  border-radius: 57px;
}
</style>