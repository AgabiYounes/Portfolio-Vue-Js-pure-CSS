<template>
  <div class="portfolio__content grid swiper-slide">
    <img
      :src="require(`@/assets/img/${portfolio.portfolio__img}`)"
      alt=""
      class="portfolio__img"
    />
    <div class="portfolio__data">
      <h3 class="portfolio__title">{{ portfolio.portfolio__title }}</h3>
      <p class="portfolio__description">
        {{ portfolio.portfolio__description }}
      </p>
      <a
        :href="portfolio.portfolio__url"
        class="button button--flex button--small portfolio__button"
        target="_blank"
        >Visit <i class="fas fa-arrow-right button__icon"></i
      ></a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Swiper",

  data() {
    return {};
  },
  props: ["portfolio"],
};
</script>
