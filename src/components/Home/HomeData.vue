<template>
  <div class="home__data">
    <h1 class="home__title">{{ home__title }}</h1>
    <h3 class="home__subtitle">{{ home__subtitle }}</h3>
    <p class="home__description">
      {{ home__description }}
    </p>
    <a href="#contact" class="button button--flex">
      {{ button__content }} <i class="far fa-paper-plane button__icon"></i>
    </a>
  </div>
</template>

<script>
export default {
  name: "HomeData",
  data() {
    return {};
  },
  props: [
    "home__description",
    "home__subtitle",
    "home__title",
    "button__content",
  ],
};
</script>