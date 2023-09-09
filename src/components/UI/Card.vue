<template>
  <div class="animal__card">
    <div class="photo">
      <img src="./../../assets/pets/image2.png" alt="" />
    </div>
    <div class="animal__info">
      <h2>MO231 - Pomeranian White</h2>
      <p><span> Gene: </span> Male <span> &#183; Age: </span>02 months</p>
      <div class="price">6.900.000 VND</div>
    </div>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.animal__card {
  padding: 8px 8px 0px 8px;
  flex-direction: column;
  align-items: flex-start;
  gap: 8px;
  border-radius: 12px;
  background: var(--neutral-color-00, #fdfdfd);
  box-shadow: 0px 4px 28px -2px rgba(0, 0, 0, 0.08);
}

.photo img {
  border-radius: 12px;
}

.animal__info {
  display: flex;
  padding: 8px 8px 20px 8px;
  flex-direction: column;
  align-items: flex-start;
}

h2 {
  color: var(--neutral-color-100, #00171f);
  font-size: 16px;
  font-weight: 700;
  line-height: 24px;
}

span {
  color: var(--neutral-color-60, #667479);
  font-size: 12px;
  font-weight: 500;
  line-height: 18px;
}

p {
  color: var(--neutral-color-60, #667479);
  font-size: 12px;
  font-weight: 700;
  line-height: 18px;
}
.price {
  color: var(--neutral-color-100, #00171f);
  font-size: 14px;
  font-weight: 700;
  line-height: 20px; 
}
</style>
