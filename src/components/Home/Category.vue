<template>
  <section class="ftco-section ftco-category ftco-no-pt">
    <div class="container">
      <div class="row">
        <div class="col-md-8">
          <div class="row">
            <div class="col-md-6 order-md-last align-items-stretch d-flex">
              <div
                class="category-wrap-2 ftco-animate img align-self-stretch d-flex vegieBanner"
              >
                <div class="text text-center">
                  <h2 class="text-capitalize">{{ title }}</h2>
                  <p>{{ descriptionTitle }}</p>
                  <p>
                    <a href="#" class="btn btn-primary">{{ shopBtn }}</a>
                  </p>
                </div>
              </div>
            </div>
            <div class="col-md-6">
              <div
                class="category-wrap ftco-animate img d-flex align-items-end"
                :class="[firstCategory.classOne, firstCategory.classTwo]"
                v-for="firstCategory in firstCategories"
                :key="firstCategory.id"
              >
                <div class="text px-3 py-1">
                  <h2 class="mb-0">
                    <a href="#" class="text-capitalize">
                      {{ firstCategory.h2 }}
                    </a>
                  </h2>
                </div>
              </div>
            </div>
          </div>
        </div>

        <div class="col-md-4">
          <div
            class="category-wrap ftco-animate img mb-4 d-flex align-items-end juices"
            :class="[secondCategory.classOne, secondCategory.classTwo]"
            v-for="secondCategory in secondCategories"
            :key="secondCategory.id"
          >
            <div class="text px-3 py-1">
              <h2 class="mb-0">
                <a href="#" class="text-capitalize">{{ secondCategory.h2 }}</a>
              </h2>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Category",
  data() {
    return {
      title: "vegetables",
      descriptionTitle: "Protect the health of every home",
      shopBtn: "Shop now",
      firstCategories: [
        { id: 1, classOne: "mb-4", classTwo: "fruits", h2: "fruit" },
        { id: 2, classTwo: "vegetables", h2: "vegetables" },
      ],
      secondCategories: [
        { id: 1, classOne: "mb-4", classTwo: "juices", h2: "juice" },
        { id: 2, classTwo: "dried", h2: "driedz" },
      ],
    };
  },
};
</script>

<style scoped>
.vegieBanner {
  background-image: url("../../assets/images/category.jpg");
}

.fruits {
  background-image: url("../../assets/images/category-1.jpg");
}

.vegetables {
  background-image: url("../../assets/images/category-2.jpg");
}

.juices {
  background-image: url("../../assets/images/category-3.jpg");
}

.dried {
  background-image: url("../../assets/images/category-4.jpg");
}
</style>
