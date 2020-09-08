<template>
  <div class="cart">
    <CartBanner />
    <CartList />
    <Newsletter />
  </div>
</template>

<script>
import CartBanner from "../components/Cart/CartBanner";
import CartList from "../components/Cart/CartList";
import Newsletter from "../components/Home/Newsletter";

export default {
  name: "Cart",
  components: {
    CartBanner,
    CartList,
    Newsletter,
  },
};
</script>
