<template>
  <div class="main-content">
    <div class="container">
      <div class="poi">
        <div v-for="(blog, i) in examples" :key="i">
          <img :src="blog.src" alt="" />
          <p>{{ blog.description }}</p>
          <p class="author">{{ blog.author }}</p>
          <img class="babge" :src="blog.date" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {
    // **************************
    // FINE COMPONETS
  },
  // **************************
  data() {
    return {
      examples: [
        {
          src: `/img/h-2-blog-img-1.jpg`,
          date: `/svg/badge.svg`,
          description: `This way, loves: a detailed guide trow new design`,
          author: `By Emily Fields`,
        },
        {
          src: `/img/h-2-blog-img-2.jpg`,
          date: `/svg/badge.svg`,
          description: `I try to give people a different way to looking art`,
          author: `By Emily Fields`,
        },
        {
          src: `/img/h-2-blog-img-3.jpg`,
          date: `/svg/badge.svg`,
          description: `Introduce Richard Laperrière of those amazing features`,
          author: `By Emily Fields`,
        },
      ],
      // **************************
      // FINE DATA E RETURN &
    };
  },
  // **************************
  computed: {
    // **************************
    // FINE COMPUTED
  },
  // **************************
  watch: {
    // **************************
    // FINE WATCH
  },
  // **************************
  methods: {
    // **************************
    // FINE METHODS
  },
  // **************************
};
</script>

<style lang="scss" scoped>
@use "../style/partials//variables" as *;
.main-content {
  width: 100%;
}
.container {
  margin: 0;
  padding: 0;
  width: 1300px;
  margin: 150px auto;
  position: relative;
}
.poi {
  display: flex;
  justify-content: space-between;
  gap: 35px;
  div {
    width: 410px;
    img {
      margin-bottom: 35px;
    }
    p {
      font-size: 21px;
    }
    .author {
      font-style: italic;
      font-weight: lighter;
      font-size: 12px;
    }
  }
}
.babge {
  width: 65px;
  position: absolute;
  z-index: 999;
  top: -25px;
  transform: translateX(16px);
}
</style>
