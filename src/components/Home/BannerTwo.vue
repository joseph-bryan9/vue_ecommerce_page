<template>
  <section class="ftco-section img">
    <div class="container">
      <div class="row justify-content-end">
        <div
          class="col-md-6 heading-section ftco-animate deal-of-the-day ftco-animate"
        >
          <span class="subheading text-capitalize">{{ subHead }}</span>
          <h2 class="mb-4">{{ h2 }}</h2>
          <p>
            {{ p }}
          </p>
          <h3><a href="#" class="text-capitalize">Spinach</a></h3>
          <span class="price"
            >{{ regPrice }} <a href="#">{{ salePrice }}</a></span
          >
          <div id="timer" class="d-flex mt-5">
            <div class="time" id="days"></div>
            <div class="time pl-3" id="hours"></div>
            <div class="time pl-3" id="minutes"></div>
            <div class="time pl-3" id="seconds"></div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BannerTwo",
  data() {
    return {
      subHead: "best price for you",
      h2: "Deal of the day",
      p:
        "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia",
      h3: "spinach",
      regPrice: "$10",
      salePrice: "now $5 only",
    };
  },
};
</script>

<style scoped>
.ftco-section {
  background-image: url("../../assets/images/bg_3.jpg");
}
</style>
