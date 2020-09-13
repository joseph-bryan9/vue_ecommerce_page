<template>
  <div class="about">
    <AboutBanner />
    <AboutContent />
    <Newsletter />
    <AboutBannerTwo />
    <Testimonials />
    <Info :style="{ backgroundColor: background}" />
  </div>
</template>

<script>
import AboutBanner from "../components/About/AboutBanner";
import AboutContent from "../components/About/AboutContent";
import Newsletter from "../components/Home/Newsletter";
import AboutBannerTwo from "../components/About/AboutBannerTwo";
import Testimonials from "../components/Home/Testimonials";
import Info from "../components/Home/Info";

export default {
  name: "About",
  components: {
    AboutBanner,
    AboutContent,
    Newsletter,
    AboutBannerTwo,
    Testimonials,
    Info,
  },
  data() {
    return {
      background: "#f7f6f2",
    };
  },
};
</script>
