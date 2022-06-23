<template>
  <div class="footer-bg py-4">
    <div class="container">
      <div class="row px-2">
        <div class="col-1 text-start p-0 pe-2">
          <h5 class="text-light">DC COMICS</h5>
          <ul class="list-unstyled">
            <li
              class="text-light text-start"
              v-for="(link, i) in dcComics"
              :key="link"
            >
              <span>{{ dcComics[i] }}</span>
            </li>
          </ul>
          <h5 class="text-light">SHOP</h5>
          <ul class="list-unstyled">
            <li
              class="text-light text-start"
              v-for="(link, i) in shop"
              :key="link"
            >
              <span>{{ shop[i] }}</span>
            </li>
          </ul>
        </div>
        <div class="col-1 text-start p-0 px-2">
          <h5 class="text-light">DC</h5>
          <ul class="list-unstyled text-start">
            <li class="text-light" v-for="(link, i) in dc" :key="link">
              <span>{{ dc[i] }}</span>
            </li>
          </ul>
        </div>
        <div class="col-1 text-start p-0 px-2">
          <h5 class="text-light">SITES</h5>
          <ul class="list-unstyled">
            <li
              class="text-light text-start"
              v-for="(link, i) in sites"
              :key="link"
            >
              <span>{{ sites[i] }}</span>
            </li>
          </ul>
        </div>
        <div class="col">
          <img
            class="dc-big-logo"
            src="/img/dc-logo-bg.png"
            alt=""
            height="400px"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TheFooter",
  data() {
    return {
      dcComics: [
        "Characters",
        "Comics",
        "Movies",
        "TV",
        "Games",
        "Videos",
        "News",
      ],
      shop: ["Shop DC", "Shop DC Collectibles"],
      dc: [
        "Terms of Use",
        "Privacy Policy (New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subscriptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
      sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa"],
      //
    };
  },
};
</script>

<style lang="scss" scoped>
.footer-bg {
  position: relative;
  overflow: hidden;
  background-image: url("/public/img/footer-bg.jpg");
  background-size: cover;
  background-position: top;
  background-repeat: no-repeat;
}
.dc-big-logo {
  position: absolute;
  top: -25%;
  right: 100px;
  height: 150%;
}
li {
  line-height: 0.9rem;
}
li span {
  font-size: 0.6rem;
  color: rgb(177, 177, 177);
}
li span:hover {
  text-decoration: underline;
  cursor: pointer;
}
</style>
