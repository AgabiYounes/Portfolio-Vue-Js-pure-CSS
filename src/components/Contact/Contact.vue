<template>
  <section class="contact section" id="contact">
    <h2 class="section__title">Contact Me</h2>
    <span class="section__subtitle">
      I'm always available to talk about my work and my projects.
    </span>
    <div class="contact__container container grid">
      <div>
        <div class="contact__information">
          <i class="fas fa-phone contact__icon"></i>
          <div>
            <h3 class="contact__title">Phone</h3>
            <span class="contact__subtitle"> +213 (0) 5 40 49 36 44 </span>
          </div>
        </div>
        <div class="contact__information">
          <i class="fas fa-envelope contact__icon"></i>
          <div>
            <h3 class="contact__title">E-Mail</h3>
            <span class="contact__subtitle"> younes.agabi03@gmail.com </span>
          </div>
        </div>
        <div class="contact__information">
          <i class="fas fa-map-marker-alt contact__icon"></i>
          <div>
            <h3 class="contact__title">Location</h3>
            <span class="contact__subtitle"> Algiers, Algeria </span>
          </div>
        </div>
      </div>
      <ContactForm></ContactForm>
    </div>
  </section>
</template>

<script>
  import ContactForm from './ContactForm.vue'
export default {
  components: {
    ContactForm
  },
  name: "Contact",

  data() {
    return {};
  },
};
</script>