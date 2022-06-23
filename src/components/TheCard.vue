<template>
  <div>
    <div class="card-image">
      <img :src="img" :alt="serie" />
    </div>
    <div class="card-body">
      <div class="card-title text-uppercase text-start">{{ serie }}</div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    img: String,
    price: String,
    serie: String,
    type: String,
  },
};
</script>

<style lang="scss" scoped>
.card-image {
  height: 160px;
  overflow: hidden;
  width: 100%;
  img {
    width: 100%;
  }
}

.card-title {
  font-size: 0.9rem;
  padding: 1rem 0;
  color: white;
}
</style>
