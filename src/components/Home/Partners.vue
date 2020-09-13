<template>
  <div>
    <hr />
    <section class="ftco-section ftco-partner">
      <div class="container">
        <div class="row">
          <div class="col-sm ftco-animate" v-for="partner in partners" :key="partner.id">
            <a href="#" class="partner">
              <img :src="partner.image" class="img-fluid" alt="Colorlib Template" />
            </a>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "Partners",
  data() {
    return {
      partners: [
        { id: 1, image: require("../../assets/images/partner-1.png") },
        { id: 2, image: require("../../assets/images/partner-2.png") },
        { id: 3, image: require("../../assets/images/partner-3.png") },
        { id: 4, image: require("../../assets/images/partner-4.png") },
        { id: 5, image: require("../../assets/images/partner-5.png") },
      ],
    };
  },
};
</script>
