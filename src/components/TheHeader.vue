<template>
  <div>
    <nav class="navbar navbar-expand-lg bg-light py-0">
      <div class="container d-flex justify-space-betwen">
        <a class="navbar-brand" href="#">
          <img src="/img/dc-logo.png" alt="" width="60" height="60" />
        </a>
        <div class="collapse navbar-collapse">
          <ul class="navbar-nav ms-auto">
            <li class="nav-item" v-for="link in navLinks" :key="link">
              <a class="nav-link active" aria-current="page" href="#">{{
                link
              }}</a>
            </li>
          </ul>
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
.nav-link:hover {
  color: rgb(70, 70, 255);
  border-bottom: 3px solid rgb(70, 70, 255);
}

.nav-item {
  font-size: 0.8rem;
}

</style>
