<template>
  <section class="ftco-section">
    <div class="container">
      <div class="row justify-content-center mb-3 pb-3">
        <div class="col-md-12 heading-section text-center ftco-animate">
          <span class="subheading text-capitalize">{{ subHeading }}</span>
          <h2 class="mb-4 text-capitalize">{{ h2 }}</h2>
          <p>
            {{ p }}
          </p>
        </div>
      </div>
    </div>
    <div class="container">
      <div class="row">
        <div
          class="col-md-6 col-lg-3 ftco-animate"
          v-for="product in products"
          :key="product"
        >
          <div class="product">
            <a href="#" class="img-prod"
              ><img
                class="img-fluid"
                :src="product.image"
                alt="Colorlib Template"
              />
              <span class="status" v-if="product.show">{{ product.sale }}</span>
              <div class="overlay"></div>
            </a>
            <div class="text py-3 pb-4 px-3 text-center">
              <h3>
                <a href="#">{{ product.h3 }}</a>
              </h3>
              <div class="d-flex">
                <div class="pricing">
                  <p class="price">
                    <span class="mr-2 price-dc" v-if="product.show">{{
                      product.ogPrice
                    }}</span
                    ><span class="price-sale">{{ product.currentPrice }}</span>
                  </p>
                </div>
              </div>
              <div class="bottom-area d-flex px-3">
                <div class="m-auto d-flex">
                  <a
                    href="#"
                    class="add-to-cart d-flex justify-content-center align-items-center text-center"
                  >
                    <span><i class="ion-ios-menu"></i></span>
                  </a>
                  <a
                    href="#"
                    class="buy-now d-flex justify-content-center align-items-center mx-1"
                  >
                    <span><i class="ion-ios-cart"></i></span>
                  </a>
                  <a
                    href="#"
                    class="heart d-flex justify-content-center align-items-center "
                  >
                    <span><i class="ion-ios-heart"></i></span>
                  </a>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Products",
  data() {
    return {
      subHeading: "featured products",
      h2: "our products",
      p:
        "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia",
      products: [
        {
          image: require("../../assets/images/product-1.jpg"),
          show: true,
          sale: "30%",
          h3: "bell pepper",
          ogPrice: "$120.00",
          currentPrice: "$80.00",
        },
        {
          image: require("../../assets/images/product-2.jpg"),
          show: false,
          h3: "strawberry",
          currentPrice: "$120.00",
        },
        {
          image: require("../../assets/images/product-3.jpg"),
          show: false,
          h3: "green beans",
          currentPrice: "$120.00",
        },
        {
          image: require("../../assets/images/product-4.jpg"),
          show: false,
          h3: "purple cabbage",
          currentPrice: "$120.00",
        },
        {
          image: require("../../assets/images/product-5.jpg"),
          show: true,
          sale: "30%",
          h3: "tomato",
          ogPrice: "$120.00",
          currentPrice: "$80.00",
        },
        {
          image: require("../../assets/images/product-6.jpg"),
          show: false,
          h3: "brocolli",
          currentPrice: "$120.00",
        },
        {
          image: require("../../assets/images/product-7.jpg"),
          show: false,
          h3: "carrots",
          currentPrice: "$120.00",
        },
        {
          image: require("../../assets/images/product-8.jpg"),
          show: false,
          h3: "fruit juice",
          currentPrice: "$120.00",
        },
      ],
    };
  },
};
</script>
