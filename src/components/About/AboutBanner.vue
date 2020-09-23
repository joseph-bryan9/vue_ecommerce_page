<template>
  <div class="hero-wrap hero-bread">
    <div class="container">
      <div class="row no-gutters slider-text align-items-center justify-content-center">
        <div class="col-md-9 ftco-animate text-center">
          <p class="breadcrumbs">
            <span class="mr-2">
              <a href="index.html">{{ link }}</a>
            </span>
            <span>{{ span }}</span>
          </p>
          <h1 class="mb-0 bread">{{ h1 }}</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AboutBanner",
  data() {
    return {
      link: "home",
      span: "About us",
      h1: "about us",
    };
  },
};
</script>

<style scoped>
.hero-bread::before {
  content: "";
}

.hero-bread {
  background-image: url("../../assets/images/bg_1.jpg");
}
</style>
