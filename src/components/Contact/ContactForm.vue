<template>
  <form class="contact__form grid" @submit.prevent="sendEmail">
    <div class="contact__inputs grid">
      <div class="contact__content">
        <label for="" class="contact__label">Name</label>
        <input
          type="text"
          class="contact__input"
          name="name"
          v-model="name"
          required
        />
      </div>
      <div class="contact__content">
        <label for="" class="contact__label">E-Mail</label>
        <input
          type="email"
          class="contact__input"
          name="email"
          v-model="email"
          required
        />
      </div>
    </div>
    <div class="contact__content">
      <label for="" class="contact__label">Project</label>
      <input
        type="text"
        class="contact__input"
        name="project"
        v-model="project"
        required
      />
    </div>
    <div class="contact__content">
      <label for="" class="contact__label">Message</label>
      <textarea
        name="message"
        cols="0"
        rows="7"
        class="contact__input"
        v-model="message"
        required
      ></textarea>
    </div>
    <div>
      <button class="button button--flex Contact__button" type="submit">
        Send Message <i class="fas fa-paper-plane button__icon"></i>
      </button>
    </div>
  </form>
</template>

<script>
import emailjs from "emailjs-com";
export default {
  components: {},
  name: "ContactForm",

  data() {
    return {
      name: "",
      email: "",
      message: "",
      project: "",
    };
  },
  methods: {
    sendEmail(e) {
      try {
        emailjs.sendForm(
          "service_2k93lxc",
          "template_28ctkki",
          e.target,
          "user_zbY5S7PSQVBFH7GpQ1sL8",
          {
            name: this.name,
            email: this.email,
            project: this.project,
            message: this.message,
          }
        );
        this.$notify({
          title: "Thank's " + this.name,
          text: "Your message has been sent successfully",
        });
      } catch (error) {
        console.log({ error });
      }

      // Reset form field
      this.name = "";
      this.email = "";
      this.message = "";
      this.project = "";
    },
  },
};
</script>