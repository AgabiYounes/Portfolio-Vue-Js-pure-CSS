<template>
  <section class="skills section" id="skills">
    <h2 class="section__title">Skills</h2>
    <span class="section__subtitle"> My Technical skills </span>
    <div class="skills__container container grid">
      <div>
        <div
          class="skills__content"
          :class="[showSkillsFrontEnd ? 'skills__open' : 'skills__close']"
        >
          <div class="skills__header" @click="showFrontEndSkills">
            <i class="fas fa-code skills__icon"></i>
            <div>
              <h1 class="skills__title">Frontend Developer</h1>
              <span class="skills__subtitle">
                More than 3 years of experience
              </span>
            </div>
            <i class="fas fa-chevron-down skills__arrow"></i>
          </div>
          <div class="skills__list grid">
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Pure CSS</h3>
                <span class="skills__number">80%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__css"></span>
              </div>
            </div>
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Bootstrap</h3>
                <span class="skills__number">90%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__bootstrap"></span>
              </div>
            </div>
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">JavaScript</h3>
                <span class="skills__number">80%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__javascript"></span>
              </div>
            </div>
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Vue.js</h3>
                <span class="skills__number">70%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__vuejs"></span>
              </div>
            </div>
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Git</h3>
                <span class="skills__number">80%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__git"></span>
              </div>
            </div>
          </div>
        </div>

        <div
          class="skills__content"
          :class="[showSkillsBackEnd ? 'skills__open' : 'skills__close']"
        >
          <div class="skills__header" @click="showBackEndSkills">
            <i class="fas fa-server skills__icon"></i>
            <div>
              <h1 class="skills__title">Backend Developer</h1>
              <span class="skills__subtitle">
                More than a year of experience
              </span>
            </div>
            <i class="fas fa-chevron-down skills__arrow"></i>
          </div>
          <div class="skills__list grid">
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Laravel</h3>
                <span class="skills__number">60%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__laravel"></span>
              </div>
            </div>
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">MySQL</h3>
                <span class="skills__number">70%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__mysql"></span>
              </div>
            </div>
          </div>
        </div>

        <div
          class="skills__content"
          :class="[showSkillsAI ? 'skills__open' : 'skills__close']"
        >
          <div class="skills__header" @click="showAISkills">
            <i class="fas fa-brain skills__icon"></i>
            <div>
              <h1 class="skills__title">AI Engineer</h1>
              <span class="skills__subtitle"> Master's degree </span>
            </div>
            <i class="fas fa-chevron-down skills__arrow"></i>
          </div>
          <div class="skills__list grid">
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Natural Language Processing</h3>
                <span class="skills__number">50%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__nlp"></span>
              </div>
            </div>
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">Python</h3>
                <span class="skills__number">80%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__python"></span>
              </div>
            </div>
            <div class="skills__data">
              <div class="skills__titles">
                <h3 class="skills__name">TensorFlow</h3>
                <span class="skills__number">60%</span>
              </div>
              <div class="skills__bar">
                <span class="skills__percentage skills__tensorflow"></span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Skills",
  components: {},
  data() {
    return {
      showSkillsFrontEnd: true,
      showSkillsBackEnd: false,
      showSkillsAI: false,
    };
  },
  methods: {
    showFrontEndSkills: function () {
      this.showSkillsFrontEnd = true;
      this.showSkillsBackEnd = false;
      this.showSkillsAI = false;
    },
    showBackEndSkills: function () {
      this.showSkillsFrontEnd = false;
      this.showSkillsBackEnd = true;
      this.showSkillsAI = false;
    },
    showAISkills: function () {
      this.showSkillsFrontEnd = false;
      this.showSkillsBackEnd = false;
      this.showSkillsAI = true;
    },
  },
};
</script>