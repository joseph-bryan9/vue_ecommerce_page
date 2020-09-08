<template>
  <div class="about">
    <AboutBanner />
    <AboutContent />
    <Newsletter />
    <AboutBannerTwo />
    <Testimonials />
  </div>
</template>

<script>
import AboutBanner from "../components/About/AboutBanner";
import AboutContent from "../components/About/AboutContent";
import Newsletter from "../components/Home/Newsletter";
import AboutBannerTwo from "../components/About/AboutBannerTwo";
import Testimonials from "../components/Home/Testimonials";

export default {
  name: "About",
  components: {
    AboutBanner,
    AboutContent,
    Newsletter,
    AboutBannerTwo,
    Testimonials,
  },
};
</script>
