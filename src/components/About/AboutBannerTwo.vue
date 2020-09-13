<template>
  <section
    class="ftco-section ftco-counter img"
    id="section-counter"
    :style="{ backgroundImage: `url(${bgImage})` }"
  >
    <div class="container">
      <div class="row justify-content-center py-5">
        <div class="col-md-10">
          <div class="row">
            <div
              class="col-md-3 d-flex justify-content-center counter-wrap ftco-animate"
              v-for="customer in customers"
              :key="customer.id"
            >
              <div class="block-18 text-center">
                <div class="text">
                  <strong class="number" data-number="10000">{{
                    customer.no
                  }}</strong>
                  <span>{{ customer.customers }}</span>
                </div>
              </div>
            </div>
            <!-- <div
              class="col-md-3 d-flex justify-content-center counter-wrap ftco-animate"
            >
              <div class="block-18 text-center">
                <div class="text">
                  <strong class="number" data-number="100">0</strong>
                  <span>Branches</span>
                </div>
              </div>
            </div>
            <div
              class="col-md-3 d-flex justify-content-center counter-wrap ftco-animate"
            >
              <div class="block-18 text-center">
                <div class="text">
                  <strong class="number" data-number="1000">0</strong>
                  <span>Partner</span>
                </div>
              </div>
            </div>
            <div
              class="col-md-3 d-flex justify-content-center counter-wrap ftco-animate"
            >
              <div class="block-18 text-center">
                <div class="text">
                  <strong class="number" data-number="100">0</strong>
                  <span>Awards</span>
                </div>
              </div>
            </div> -->
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutBannerTwo",
  data() {
    return {
      bgImage: require("../../assets/images/bg_3.jpg"),
      customers: [
        { id: 1, no: "10,000", customers: "happy customers" },
        { id: 2, no: "100", customers: "branches" },
        { id: 3, no: "1,000", customers: "partners" },
        { id: 4, no: "100", customers: "awards" },
      ],
    };
  },
};
</script>
