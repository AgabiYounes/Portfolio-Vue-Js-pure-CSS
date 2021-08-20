<template>
  <header
    class="header"
    id="header"
    :class="{ scroll__header: scrollPosition >= 80 }"
  >
    <NavBar></NavBar>
  </header>
</template>

<script>
// @ is an alias to /src
import NavBar from "./NavBar";

export default {
  name: "Header",
  components: {
    NavBar,
  },
  data() {
    return {
      scrollPosition: null,
    };
  },
  methods: {
    updateScroll() {
      this.scrollPosition = window.scrollY;
    },
  },
  mounted() {
    window.addEventListener("scroll", this.updateScroll);
  },
};
</script>
