<template>
  <div class="py-1 bg-primary">
    <div class="container">
      <div
        class="row no-gutters d-flex align-items-start align-items-center px-md-0"
      >
        <div class="col-lg-12 d-block">
          <div class="row d-flex">
            <div class="col-md pr-4 d-flex topper align-items-center">
              <div
                class="icon mr-2 d-flex justify-content-center align-items-center"
              >
                <span class="icon-phone2"></span>
              </div>
              <span class="text">{{ mobileNo }}</span>
            </div>
            <div class="col-md pr-4 d-flex topper align-items-center">
              <div
                class="icon mr-2 d-flex justify-content-center align-items-center"
              >
                <span class="icon-paper-plane"></span>
              </div>
              <span class="text">{{ email }}</span>
            </div>
            <div
              class="col-md-5 pr-4 d-flex topper align-items-center text-lg-right"
            >
              <span class="text">{{ notice }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      mobileNo: "+ 1235 2355 98",
      email: "youremail@email.com",
      notice: "3-5 Business days delivery & Free Returns",
    };
  },
};
</script>
