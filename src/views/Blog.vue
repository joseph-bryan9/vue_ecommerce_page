<template>
  <div class="Blog">
    <BlogBanner />
    <BlogPosts />
  </div>
</template>

<script>
import BlogBanner from "../components/Blog/BlogBanner";
import BlogPosts from "../components/Blog/BlogPosts";

export default {
  name: "Blog",
  components: {
    BlogBanner,
    BlogPosts,
  },
};
</script>
