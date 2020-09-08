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
              <h1 class="mb-2">We serve Fresh Vegestables &amp; Fruits</h1>
              <h2 class="subheading mb-4">
                We deliver organic vegetables &amp; fruits
              </h2>
              <p>
                <a href="#" class="btn btn-primary">View Details</a>
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

<style scoped>
.sliderOne {
  background: url("../../assets/images/bg_1.jpg");
}

.ftco-animate {
  opacity: 1;
  visibility: visible;
}

/* .sliderTwo {
  background: url("../../assets/images/bg_2.jpg");
} */

.owl-carousel {
  display: block;
}
</style>
