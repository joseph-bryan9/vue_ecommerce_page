<template>
  <div id="app" class="goto-here">
    <Header />
    <Navigation />
    <router-view />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header";
import Navigation from "./components/Navigation";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    Header,
    Navigation,
    Footer,
  },
};
</script>

<style>
.ftco-animate {
  opacity: 1;
  visibility: visible;
}

.owl-carousel {
  display: flex;
}
</style>
