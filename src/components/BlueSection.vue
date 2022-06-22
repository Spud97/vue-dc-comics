<template>
  <div class="bg-primary">
    <div class="container">
      <div class="row py-5 align-items-center">
        <div v-for="link in blueSectionLinks" :key="link.text" class="col">
          <a href="#" class="row align-items-center">
            <img
              class="col-auto pe-0"
              :src="`/img/buy-${link.icon}`"
              :alt="`Immagine ` + link.text"
            />
            <span class="col text-white text-uppercase ps-0">{{ link.text }}</span>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      blueSectionLinks: [
        {
          text: "Digital Comics",
          icon: "comics-digital-comics.png",
        },
        {
          text: "DC Merchandise",
          icon: "comics-merchandise.png",
        },
        {
          text: "Subscription",
          icon: "comics-subscriptions.png",
        },
        {
          text: "Comic Shop Locator",
          icon: "comics-shop-locator.png",
        },
        {
          text: "DC power Visa",
          icon: "dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
span {
  font-size: 0.8rem;
}
a {
    text-decoration: none;
}
img {
  transform: scale(0.7) translateX(3rem);
  max-width: 90px;
  max-height: 70px;
}
</style>
