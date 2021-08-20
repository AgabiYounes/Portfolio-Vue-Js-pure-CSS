<template>
  <section class="project section">
    <div class="project__bg">
      <div class="project__container container grid">
        <div class="project__data">
          <h2 class="project__title">You have a new project!</h2>
          <p class="project__description">
            You want to realize a new project and you are looking for a web
            developer? Realize your dreams by contacting me 😄.
          </p>
          <a href="#contact" class="button button--flex button--white">
            Contact Me
            <i class="fas fa-paper-plane project__icon button__icon"></i
          ></a>
        </div>
        <img src="@/assets/img/younes.png" alt="" class="project__img" />
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "Project",

  data() {
    return {};
  },
};
</script>