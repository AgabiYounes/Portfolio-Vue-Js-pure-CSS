<template>
  <section class="about section" id="about">
    <h2 class="section__title">About Me</h2>
    <span class="section__subtitle"> My introduction </span>
    <div class="about__container container grid">
      <img src="~@/assets/img/about.jpg" alt="" class="about__img" />
      <div class="about__data">
        <p class="about__description">
          My name's <strong>Younes AGABI</strong>. I am an
          <strong>artificial intelligence engineer</strong> and a
          <strong>front-end developer</strong> with <strong>+3 years</strong> of
          experience. I did my internship at the University of Deakin in
          Australia and i'm interested in UI & UX Web Design trends. I mainly
          use <strong>Vue js</strong> to realize my web projects as well as some
          knowledge in <strong>Laravel</strong> for the BackEnd. I like to make
          fun and interactive things with code because in the end, there are
          three possible reactions to any design: yes, no and
          <strong>WAHOU!</strong>, the third one is the one I'm aiming for.
        </p>
        <div class="about__info">
          <div>
            <span class="about__info-title">+3</span>
            <span class="about__info-name"
              >Years <br />
              experience</span
            >
          </div>
          <div>
            <span class="about__info-title">+6</span>
            <span class="about__info-name"
              >Completed <br />
              project</span
            >
          </div>
          <div>
            <span class="about__info-title">2</span>
            <span class="about__info-name"
              >Companies <br />
              worked</span
            >
          </div>
        </div>
        <div class="about__buttons">
          <a
            href="https://www.canva.com/design/DAEZAM_I9ZM/RbwJy0kEKYsMRNkYbQaT8A/view?utm_content=DAEZAM_I9ZM&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink"
            class="button button--flex"
            target="_blank"
          >
            Download CV<i class="fas fa-download button__icon"></i>
          </a>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "About",
  components: {},
  data() {
    return {};
  },
};
</script>