<template>
  <section class="ftco-section">
    <div class="container">
      <div class="row no-gutters ftco-services">
        <div
          class="col-md-3 text-center d-flex align-self-stretch ftco-animate"
          v-for="icon in icons"
          :key="icon.id"
        >
          <div class="media block-6 services mb-md-0 mb-4">
            <div
              class="icon active d-flex justify-content-center align-items-center mb-2"
              :class="icon.bgColor"
            >
              <span class="flaticon-shipped" :class="icon.class"></span>
            </div>
            <div class="media-body">
              <h3 class="heading">{{ icon.h3 }}</h3>
              <span>{{ icon.span }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Info",
  data() {
    return {
      icons: [
        {
          id: 1,
          bgColor: "bg-color-1",
          class: "flaticon-shipped",
          h3: "free shipping",
          span: "on order over $100",
        },
        {
          id: 2,
          bgColor: "bg-color-2",
          class: "flaticon-diet",
          h3: "always fresh",
          span: "product well package",
        },
        {
          id: 3,
          bgColor: "bg-color-3",
          class: "flaticon-award",
          h3: "superior quality",
          span: "quality products",
        },
        {
          id: 4,
          bgColor: "bg-color-4",
          class: "flaticon-customer-service",
          h3: "support",
          span: "24/7 support",
        },
      ],
    };
  },
};
</script>
