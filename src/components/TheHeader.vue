<template>
  <div>
    <nav class="navbar navbar-expand-lg bg-light py-0">
      <div class="container d-flex justify-content-betwen">
        <a class="navbar-brand" href="#">
          <img
            src="/img/dc-logo.png"
            alt=""
            width="60"
            height="60"
            class="my-2"
          />
        </a>
        <div id="box-link" class="d-flex">
          <div v-for="link in navLinks" :key="link" class="h-100">
            <a class="nav-link active bold d-flex align-items-center" aria-current="page" href="#">{{
              link
            }}</a>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "TheHeader",
  data() {
    return {
      navLinks: [
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP",
      ],
      //
    };
  },
  components: {},
};
</script>

<style lang="scss" scoped>
#box-link {
  height: 86px;
}
.nav-link {
  padding: 10px 15px;
  font-weight: bold;
  font-size: 0.8rem;
  height: 100%;
}
.nav-link:hover {
  color: rgb(70, 70, 255);
  border-bottom: 3px solid rgb(70, 70, 255);
}
</style>
