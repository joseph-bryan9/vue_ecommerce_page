<template>
  <section id="home-section" class="hero">
    <div class="home-slider owl-carousel">
      <div class="slider-item sliderOne">
        <div class="overlay"></div>
        <div class="container">
          <div
            class="row slider-text justify-content-center align-items-center"
            data-scrollax-parent="true"
          >
            <div class="col-md-12 ftco-animate text-center">
              <h1 class="mb-2">{{ h1 }}</h1>
              <h2 class="subheading mb-4">
                {{ h2 }}
              </h2>
              <p>
                <a href="#" class="btn btn-primary">{{ btn }}</a>
              </p>
            </div>
          </div>
        </div>
      </div>

      <!-- <div class="slider-item sliderTwo">
        <div class="overlay"></div>
        <div class="container">
          <div
            class="row slider-text justify-content-center align-items-center"
            data-scrollax-parent="true"
          >
            <div class="col-sm-12 ftco-animate text-center">
              <h1 class="mb-2">100% Fresh &amp; Organic Foods</h1>
              <h2 class="subheading mb-4">
                We deliver organic vegetables &amp; fruits
              </h2>
              <p>
                <a href="#" class="btn btn-primary">View Details</a>
              </p>
            </div>
          </div>
        </div>
      </div> -->
    </div>
  </section>
</template>

<script>
export default {
  name: "Banner",
  data() {
    return {
      h1: "we serve fresh vegetables & fruits",
      h2: "we deliver organic vegetables & fruits",
      btn: "view details",
    };
  },
};
</script>

<style scoped>
.sliderOne {
  background: url("../../assets/images/bg_1.jpg");
}

.ftco-animate {
  opacity: 1;
  visibility: visible;
}

.owl-carousel {
  display: block;
}

.owl-carousel.home-slider .slider-item .overlay {
  opacity: 0.4;
}

.owl-carousel.home-slider .slider-item .slider-text h1 {
  text-shadow: 5px 3px 8px #000;
}

.owl-carousel.home-slider .slider-item .slider-text .subheading {
  font-size: 16px;
  text-shadow: 5px 3px 8px #000;
}

.btn.btn-primary:hover {
  background: #fff;
}
</style>
