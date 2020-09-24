<template>
  <div
    class="hero-wrap hero-bread"
    style="background-image: url('../../assets/images/bg_1.jpg');"
    :style="{ backgroundImage: `url(${bgImage})` }"
  >
    <div class="container">
      <div
        class="row no-gutters slider-text align-items-center justify-content-center"
      >
        <div class="col-md-9 ftco-animate text-center">
          <p class="breadcrumbs">
            <span class="mr-2 text-capitalize"
              ><a href="index.html">{{ link }}</a></span
            >
            <span class="text-capitalize">{{ span }}</span>
          </p>
          <h1 class="mb-0 bread text-capitalize">{{ h1 }}</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CartBanner",
  data() {
    return {
      bgImage: require("../../assets/images/bg_1.jpg"),
      link: "home",
      span: "cart",
      h1: "my carts",
    };
  },
};
</script>
