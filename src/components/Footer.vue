<template>
  <footer class="ftco-footer ftco-section">
    <div class="container">
      <div class="row">
        <div class="mouse">
          <a href="#" class="mouse-icon">
            <div class="mouse-wheel">
              <span class="ion-ios-arrow-up"></span>
            </div>
          </a>
        </div>
      </div>
      <div class="row mb-5">
        <div class="col-md">
          <div class="ftco-footer-widget mb-4">
            <h2 class="ftco-heading-2 text-capitalize">{{ brandname }}</h2>
            <p>
              {{ p }}
            </p>
            <ul
              class="ftco-footer-social list-unstyled float-md-left float-lft mt-5"
            >
              <li class="ftco-animate" v-for="icon in icons" :key="icon">
                <a href="#">
                  <span :class="icon.socialIcon"></span>
                </a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-md">
          <div class="ftco-footer-widget mb-4 ml-md-5">
            <h2 class="ftco-heading-2 text-capitalize">{{ menuTitle }}</h2>
            <ul class="list-unstyled">
              <li v-for="menuList in menuLists" :key="menuList">
                <a href="#" class="py-2 d-block text-capitalize">{{
                  menuList.menu
                }}</a>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-md-4">
          <div class="ftco-footer-widget mb-4">
            <h2 class="ftco-heading-2 text-capitalize">{{ helpTitle }}</h2>
            <div class="d-flex">
              <ul class="list-unstyled mr-l-5 pr-l-3 mr-4">
                <li v-for="helpListOne in helpListsOne" :key="helpListOne">
                  <a href="#" class="py-2 d-block text-capitalize">{{
                    helpListOne.helpInfo
                  }}</a>
                </li>
              </ul>
              <ul class="list-unstyled">
                <li v-for="helpListTwo in helpListsTwo" :key="helpListTwo">
                  <a href="#" class="py-2 d-block text-capitalize">{{
                    helpListTwo.helpInfo
                  }}</a>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-md">
          <div class="ftco-footer-widget mb-4">
            <h2 class="ftco-heading-2">{{ questionTitle }}</h2>
            <div class="block-23 mb-3">
              <ul>
                <li>
                  <span class="icon icon-map-marker"></span>
                  <span class="text">{{ address }}</span>
                </li>
                <li>
                  <a href="#">
                    <span class="icon icon-phone"></span>
                    <span class="text">{{ contactNo }}</span>
                  </a>
                </li>
                <li>
                  <a href="#">
                    <span class="icon icon-envelope"></span>
                    <span class="text">{{ email }}</span>
                  </a>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-12 text-center">
          <p>
            <!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
            {{ copyrightPOne }} &copy;
            {{ new Date().getFullYear() }}
            {{ copyrightPTwo }} by
            <a href="https://josephbryansena.com" target="_blank">{{
              joseph
            }}</a>
            <!-- Link back to Colorlib can't be removed. Template is licensed under CC BY 3.0. -->
          </p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      // First Column
      brandname: "vegefoods",
      p:
        "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia.",
      icons: [
        { socialIcon: "icon-twitter" },
        { socialIcon: "icon-facebook" },
        { socialIcon: "icon-instagram" },
      ],
      // Second Column
      menuTitle: "menu",
      menuLists: [
        { menu: "shop" },
        { menu: "about" },
        { menu: "journal" },
        { menu: "contact us" },
      ],
      // Third Column
      helpTitle: "help",
      helpListsOne: [
        { helpInfo: "shipping information" },
        { helpInfo: "returns & exchange" },
        { helpInfo: "terms & conditions" },
        { helpInfo: "privacy policy" },
      ],
      helpListsTwo: [{ helpInfo: "FAQs" }, { helpInfo: "contact" }],
      // Fourth Column
      questionTitle: "Have a Question?",
      address: "203 Fake St. Mountain View, San Francisco, California, USA",
      contactNo: "+2 392 3929 210",
      email: "info@yourdomain.com",
      // Copyright row
      copyrightPOne: "Copyright",
      copyrightPTwo: "All rights reserved | This template is revised",
      joseph: "Joseph Seña",
    };
  },
};
</script>
