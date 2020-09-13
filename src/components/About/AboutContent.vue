<template>
  <section class="ftco-section ftco-no-pb ftco-no-pt bg-light">
    <div class="container">
      <div class="row">
        <div
          class="col-md-5 p-md-5 img img-2 d-flex justify-content-center align-items-center"
          :style="{ backgroundImage: `url(${bgImage})` }"
        >
          <a
            :href="video"
            class="icon popup-vimeo d-flex justify-content-center align-items-center"
          >
            <span class="icon-play"></span>
          </a>
        </div>
        <div class="col-md-7 py-5 wrap-about pb-md-5 ftco-animate">
          <div class="heading-section-bold mb-4 mt-md-5">
            <div class="ml-md-0">
              <h2 class="mb-4">{{ h2 }}</h2>
            </div>
          </div>
          <div class="pb-md-5">
            <p>{{ p1 }}</p>
            <p>
              {{ p2 }}
            </p>
            <p>
              <a href="#" class="btn btn-primary">{{ shopBtn }}</a>
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "AboutContent",
  data() {
    return {
      bgImage: require("../../assets/images/about.jpg"),
      video: "https://vimeo.com/45830194",
      h2: "Welcome to Vegefoods an eCommerce website",
      p1:
        "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean.",
      p2:
        "But nothing the copy said could convince her and so it didn’t take long until a few insidious Copy Writers ambushed her, made her drunk with Longe and Parole and dragged her into their agency, where they abused her for their.",
      shopBtn: "Shop now",
    };
  },
};
</script>
