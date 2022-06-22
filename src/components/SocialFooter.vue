<template>
  <div class="bg-dark">
    <div class="container">
      <div class="d-flex justify-content-between align-items-center">
        <div>
          <button type="button" class="btn btn-outline-primary my-btn">
            SIGN-UP NOW!
          </button>
        </div>
        <div class="d-flex align-items-center">
          <ul
            class="list-unstyled d-flex justify-content-between align-items-center"
          >
            <li class="p-4 text-primary fw-bold">FOLLOW US</li>
            <li class="m-3">
              <a href="#"> <img src="/img/footer-facebook.png" alt="" /></a>
            </li>

            <li class="m-3">
              <a href="#"><img src="/img/footer-twitter.png" alt="" /></a>
            </li>

            <li class="m-3">
              <a href="#"><img src="/img/footer-youtube.png" alt="" /></a>
            </li>

            <li class="m-3">
              <a href="#"><img src="/img/footer-pinterest.png" alt="" /></a>
            </li>

            <li class="m-3">
              <a href="#"><img src="/img/footer-periscope.png" alt="" /></a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SocialFooter",
  data() {
    return {
      //
    };
  },
  components: {},
};
</script>

<style lang="scss" scoped>
.my-btn {
  border-radius: 0px;
  color: white;
}
</style>
