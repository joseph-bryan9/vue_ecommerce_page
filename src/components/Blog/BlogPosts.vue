<template>
  <section class="ftco-section ftco-degree-bg">
    <div class="container">
      <div class="row">
        <div class="col-lg-8 ftco-animate">
          <div class="row">
            <div class="col-md-12 d-flex ftco-animate" v-for="blog in blogs" :key="blog.id">
              <div class="blog-entry align-self-stretch d-md-flex">
                <a
                  href="blog-single.html"
                  class="block-20"
                  :style="{ backroundImage: `url(${blog.bgImage})` }"
                ></a>
                <div class="text d-block pl-md-4">
                  <div class="meta mb-3">
                    <div>
                      <a href="#" class="text-capitalize">{{ blog.date }}</a>
                    </div>
                    <div>
                      <a href="#" class="text-capitalize">{{ blog.author }}</a>
                    </div>
                    <div>
                      <a href="#" class="meta-chat">
                        <span class="icon-chat"></span>
                        {{ blog.commentCount }}
                      </a>
                    </div>
                  </div>
                  <h3 class="heading">
                    <a href="#">{{ blog.link }}</a>
                  </h3>
                  <p>{{ blog.p }}</p>
                  <p>
                    <a href="blog-single.html" class="btn btn-primary py-2 px-3">{{ blog.readBtn }}</a>
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- .col-md-8 -->
        <div class="col-lg-4 sidebar ftco-animate">
          <div class="sidebar-box">
            <form action="#" class="search-form">
              <div class="form-group">
                <span class="icon ion-ios-search"></span>
                <input type="text" class="form-control" placeholder="Search..." />
              </div>
            </form>
          </div>
          <div class="sidebar-box ftco-animate">
            <h3 class="heading text-capitalize">{{ h3Category }}</h3>
            <ul class="categories">
              <li v-for="category in categories" :key="category.id">
                <a href="#" class="text-capitalize">
                  {{ category.name }}
                  <span>{{ category.qty }}</span>
                </a>
              </li>
            </ul>
          </div>

          <div class="sidebar-box ftco-animate">
            <h3 class="heading text-capitalize">{{ h3Blog }}</h3>
            <div
              class="block-21 mb-4 d-flex"
              v-for="recentBlog in recentBlogs"
              :key="recentBlog.id"
            >
              <a
                class="blog-img mr-4"
                style="background-image: url(../../assets/images/image_1.jpg);"
                :style="{ backroundImage: `url(${recentBlog.bgImage})` }"
              ></a>
              <div class="text">
                <h3 class="heading-1">
                  <a href="#">{{ link }}</a>
                </h3>
                <div class="meta">
                  <div>
                    <a href="#">
                      <span class="icon-calendar"></span>
                      {{ date }}
                    </a>
                  </div>
                  <div>
                    <a href="#">
                      <span class="icon-person"></span>
                      {{ author }}
                    </a>
                  </div>
                  <div>
                    <a href="#">
                      <span class="icon-chat"></span>
                      {{ commentCount }}
                    </a>
                  </div>
                </div>
              </div>
            </div>
            <!-- <div class="block-21 mb-4 d-flex">
              <a
                class="blog-img mr-4"
                style="background-image: url(../../assets/images/image_2.jpg);"
              ></a>
              <div class="text">
                <h3 class="heading-1">
                  <a href="#"
                    >Even the all-powerful Pointing has no control about the
                    blind texts</a
                  >
                </h3>
                <div class="meta">
                  <div>
                    <a href="#"
                      ><span class="icon-calendar"></span> April 09, 2019</a
                    >
                  </div>
                  <div>
                    <a href="#"><span class="icon-person"></span> Admin</a>
                  </div>
                  <div>
                    <a href="#"><span class="icon-chat"></span> 19</a>
                  </div>
                </div>
              </div>
            </div>
            <div class="block-21 mb-4 d-flex">
              <a
                class="blog-img mr-4"
                style="background-image: url(../../assets/images/image_3.jpg);"
              ></a>
              <div class="text">
                <h3 class="heading-1">
                  <a href="#"
                    >Even the all-powerful Pointing has no control about the
                    blind texts</a
                  >
                </h3>
                <div class="meta">
                  <div>
                    <a href="#"
                      ><span class="icon-calendar"></span> April 09, 2019</a
                    >
                  </div>
                  <div>
                    <a href="#"><span class="icon-person"></span> Admin</a>
                  </div>
                  <div>
                    <a href="#"><span class="icon-chat"></span> 19</a>
                  </div>
                </div>
              </div>
            </div>-->
          </div>

          <div class="sidebar-box ftco-animate">
            <h3 class="heading text-capitalize">{{ h3Food }}</h3>
            <div class="tagcloud">
              <a
                href="#"
                class="tag-cloud-link"
                v-for="food in foods"
                :key="food.id"
              >{{ food.food }}</a>
              <!-- <a href="#" class="tag-cloud-link">tomatoe</a>
              <a href="#" class="tag-cloud-link">mango</a>
              <a href="#" class="tag-cloud-link">apple</a>
              <a href="#" class="tag-cloud-link">carrots</a>
              <a href="#" class="tag-cloud-link">orange</a>
              <a href="#" class="tag-cloud-link">pepper</a>
              <a href="#" class="tag-cloud-link">eggplant</a>-->
            </div>
          </div>

          <div class="sidebar-box ftco-animate">
            <h3 class="heading text-capitalize">{{ h3Paragraph }}</h3>
            <p>{{ p }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "BlogPosts",
  data() {
    return {
      blogs: [
        {
          id: 1,
          bgImage: require("../../assets/images/image_1.jpg"),
          date: "july 20, 2019",
          author: "admin",
          commentCount: 3,
          link:
            "Even the all-powerful Pointing has no control about the blind texts",
          p:
            "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          readBtn: "Read more",
        },
        {
          id: 2,
          bgImage: require("../../assets/images/image_2.jpg"),
          date: "july 12, 2019",
          author: "admin",
          commentCount: 6,
          link:
            "Even the all-powerful Pointing has no control about the blind texts",
          p:
            "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          readBtn: "Read more",
        },
        {
          id: 3,
          bgImage: require("../../assets/images/image_3.jpg"),
          date: "june 28, 2019",
          author: "admin",
          commentCount: 8,
          link:
            "Even the all-powerful Pointing has no control about the blind texts",
          p:
            "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          readBtn: "Read more",
        },
        {
          id: 4,
          bgImage: require("../../assets/images/image_4.jpg"),
          date: "june 15, 2019",
          author: "admin",
          commentCount: 2,
          link:
            "Even the all-powerful Pointing has no control about the blind texts",
          p:
            "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          readBtn: "Read more",
        },
        {
          id: 5,
          bgImage: require("../../assets/images/image_5.jpg"),
          date: "june 10, 2019",
          author: "admin",
          commentCount: 4,
          link:
            "Even the all-powerful Pointing has no control about the blind texts",
          p:
            "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          readBtn: "Read more",
        },
        {
          id: 6,
          bgImage: require("../../assets/images/image_6.jpg"),
          date: "may 25, 2019",
          author: "admin",
          commentCount: 9,
          link:
            "Even the all-powerful Pointing has no control about the blind texts",
          p:
            "Far far away, behind the word mountains, far from the countries Vokalia and Consonantia, there live the blind texts.",
          readBtn: "Read more",
        },
      ],
      h3Category: "categories",
      categories: [
        { id: 1, name: "vegetables", qty: "(12)" },
        { id: 2, name: "fruits", qty: "(22)" },
        { id: 3, name: "juice", qty: "(37)" },
        { id: 4, name: "dries", qty: "(42)" },
      ],
      h3Blog: "recent blog",
      recentBlogs: [
        {
          id: 1,
          bgImage: require("../../assets/images/image_1.jpg"),
          link:
            "Even the all-powerful Pointing has no control about the blind texts",
          date: "April 09, 2019",
          author: "Admin",
          commentCount: 19,
        },
        {
          id: 2,
          bgImage: require("../../assets/images/image_2.jpg"),
          link:
            "Even the all-powerful Pointing has no control about the blind texts",
          date: "April 09, 2019",
          author: "Admin",
          commentCount: 19,
        },
        {
          id: 3,
          bgImage: require("../../assets/images/image_3.jpg"),
          link:
            "Even the all-powerful Pointing has no control about the blind texts",
          date: "April 09, 2019",
          author: "Admin",
          commentCount: 19,
        },
      ],
      h3Food: "tag cloud",
      foods: [
        { id: 1, food: "fruits" },
        { id: 2, food: "tomato" },
        { id: 3, food: "mango" },
        { id: 4, food: "apple" },
        { id: 5, food: "carrot" },
        { id: 6, food: "orange" },
        { id: 7, food: "pepper" },
        { id: 8, food: "eggplant" },
      ],
      h3Paragraph: "paragraph",
      p:
        "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ducimus itaque, autem necessitatibus voluptate quod mollitia delectus aut, sunt placeat nam vero culpa sapiente consectetur similique, inventore eos fugit cupiditate numquam!",
    };
  },
};
</script>
