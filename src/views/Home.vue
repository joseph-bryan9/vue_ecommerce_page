<template>
  <div class="home">
    <Banner />
    <Info />
    <Category />
    <Products />
    <BannerTwo />
    <Testimonials />
    <Partners />
    <Newsletter />
  </div>
</template>

<script>
// @ is an alias to /src
import Banner from "../components/Home/Banner";
import Info from "../components/Home/Info";
import Category from "../components/Home/Category";
import Products from "../components/Home/Products";
import BannerTwo from "../components/Home/BannerTwo";
import Testimonials from "../components/Home/Testimonials";
import Partners from "../components/Home/Partners";
import Newsletter from "../components/Home/Newsletter";

export default {
  name: "Home",
  components: {
    Banner,
    Info,
    Category,
    Products,
    BannerTwo,
    Testimonials,
    Partners,
    Newsletter,
  },
};
</script>
