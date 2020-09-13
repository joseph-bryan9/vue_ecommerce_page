<template>
  <div>
    <section class="ftco-section testimony-section">
      <div class="container">
        <div class="row justify-content-center mb-5 pb-3">
          <div class="col-md-7 heading-section ftco-animate text-center">
            <span class="subheading text-capitalize">{{ subHead }}</span>
            <h2 class="mb-4">{{ h2 }}</h2>
            <p>{{ p }}</p>
          </div>
        </div>
        <div class="row ftco-animate">
          <div class="col-md-12">
            <div class="carousel-testimony owl-carousel">
              <div class="item" v-for="client in clients" :key="client.id">
                <div class="testimony-wrap p-4 pb-5">
                  <div class="user-img mb-5" :style="{ backgroundImage: `url(${client.image})` }">
                    <span class="quote d-flex align-items-center justify-content-center">
                      <i class="icon-quote-left"></i>
                    </span>
                  </div>
                  <div class="text text-center">
                    <p class="mb-5 pl-4 line">{{ client.p }}</p>
                    <p class="name text-capitalize">{{ client.name }}</p>
                    <span class="position text-capitalize">
                      {{
                      client.position
                      }}
                    </span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "Testimonials",
  data() {
    return {
      subHead: "testimony",
      h2: "Our satisfied customer says",
      p:
        "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in",
      clients: [
        {
          id: 1,
          image: require("../../assets/images/person_1.jpg"),
          p:
            "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          name: "garreth smith",
          position: "marketing manager",
        },
        {
          id: 2,
          image: require("../../assets/images/person_2.jpg"),
          p:
            "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          name: "grayson johnsons",
          position: "interface manager",
        },
        {
          id: 3,
          image: require("../../assets/images/person_3.jpg"),
          p:
            "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          name: "karl longley",
          position: "ui designer",
        },
      ],
    };
  },
};
</script>
