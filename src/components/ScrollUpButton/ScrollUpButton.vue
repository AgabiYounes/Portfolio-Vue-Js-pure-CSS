<template>
  <a
    href="#"
    class="scrollup"
    id="scrollup"
    :class="{ show__scroll: scrollPositionScroll >= 560 }"
  >
    <i class="fas fa-arrow-up scrollup__icon"></i>
  </a>
</template>
<script>
export default {
  name: "ScrollUpButton",

  data() {
    return {
      scrollPositionScroll: null,
    };
  },
  methods: {
    updateScrollScroll() {
      this.scrollPositionScroll = window.scrollY;
    },
  },
  mounted() {
    window.addEventListener("scroll", this.updateScrollScroll);
  },
};
</script>