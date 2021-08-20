<template>
  <footer class="footer">
    <div class="footer__bg">
      <div class="footer__container container grid">
        <div>
          <h1 class="footer__title">Younes</h1>
          <span class="footer__subtitle">Frontend Developer</span>
        </div>
        <ul class="footer__links">
          <li>
            <a href="#skills" class="footer__link">Skills</a>
          </li>
          <li>
            <a href="#qualification" class="footer__link">Qualification</a>
          </li>
          <li>
            <a href="#portfolio" class="footer__link">Portfolio</a>
          </li>
          <li>
            <a href="#contact" class="footer__link">Contact</a>
          </li>
        </ul>
        <div class="footer__socials">
          <a
            href="https://github.com/AgabiYounes"
            class="footer__social"
            target="_blank"
          >
            <i class="fab fa-github"></i
          ></a>
          <a
            href="https://www.linkedin.com/in/younes-agabi/"
            class="footer__social"
            target="_blank"
          >
            <i class="fab fa-linkedin"></i
          ></a>
          <a
            href="https://www.facebook.com/younes.agabi"
            class="footer__social"
            target="_blank"
          >
            <i class="fab fa-facebook"></i
          ></a>
        </div>
      </div>

      <p class="footer__copy">No rights reserved, you can use it 😁</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",

  data() {
    return {};
  },
};
</script>