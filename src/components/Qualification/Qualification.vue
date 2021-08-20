<template>
  <section class="qualification section" id="qualification">
    <h2 class="section__title">Qualification</h2>
    <span class="section__subtitle">My personnal journey</span>
    <div class="qualification__container container">
      <div class="qualification__tabs">
        <div
          class="qualification__button button--flex"
          @click="showEducationFunction"
          :class="{ 'qualification__active-button': showEducation }"
        >
          <i class="fas fa-graduation-cap qualification__icon"></i> Education
        </div>
        <div
          class="qualification__button button--flex"
          @click="showInternshipFunction"
          :class="{ 'qualification__active-button': showInternship }"
        >
          <i class="fas fa-address-card qualification__icon"></i> Internship
        </div>
        <div
          class="qualification__button button--flex"
          @click="showWorkFunction"
          :class="{ 'qualification__active-button': showWork }"
        >
          <i class="fas fa-briefcase qualification__icon"></i> Work
        </div>
      </div>
      <div class="qualification__sections">
        <div
          class="qualification__content"
          data-content
          id="education"
          :class="{ qualification__active: showEducation }"
        >
          <div class="qualification__data">
            <div>
              <h3 class="qualification__title">
                Artificial Intelligence Engineer
              </h3>
              <span class="qualification__subtitle">
                Master's degree - University of Algiers, Algeria
              </span>
              <div class="qualification__calendar">
                <i class="far fa-calendar"></i> 2018 - 2020
              </div>
            </div>

            <div>
              <span class="qualification__rounded"> </span>
              <span class="qualification__line"> </span>
            </div>
          </div>

          <div class="qualification__data">
            <div></div>
            <div>
              <span class="qualification__rounded"> </span>
            </div>
            <div>
              <h3 class="qualification__title">Computer systems</h3>
              <span class="qualification__subtitle">
                Bachelor's degree - University of Algiers, Algeria
              </span>
              <div class="qualification__calendar">
                <i class="far fa-calendar"></i> 2015 - 2018
              </div>
            </div>
          </div>
        </div>

        <div
          class="qualification__content"
          data-content
          id="work"
          :class="{ qualification__active: showWork }"
        >
          <div class="qualification__data">
            <div>
              <h3 class="qualification__title">Frontend Developer</h3>
              <span class="qualification__subtitle"> ADEX Technology </span>
              <div class="qualification__calendar">
                <i class="far fa-calendar"></i> 2021 - Present
              </div>
            </div>
            <div>
              <span class="qualification__rounded"> </span>
              <span class="qualification__line"> </span>
            </div>
          </div>

          <div class="qualification__data">
            <div></div>
            <div>
              <span class="qualification__rounded"> </span>
              <span class="qualification__line"> </span>
            </div>
            <div>
              <h3 class="qualification__title">
                Techno-functional ERP Consultant
              </h3>
              <span class="qualification__subtitle"> Atom Algeria </span>
              <div class="qualification__calendar">
                <i class="far fa-calendar"></i> 2020 - 2021
              </div>
            </div>
          </div>
          <div class="qualification__data">
            <div>
              <h3 class="qualification__title">Web Developer</h3>
              <span class="qualification__subtitle"> Digitalex </span>
              <div class="qualification__calendar">
                <i class="far fa-calendar"></i> 2017
              </div>
            </div>
            <div>
              <span class="qualification__rounded"> </span>
            </div>
          </div>
        </div>
        <div
          class="qualification__content"
          data-content
          id="intership"
          :class="{ qualification__active: showInternship }"
        >
          <div class="qualification__data">
            <div>
              <h3 class="qualification__title">End-Of-Degree Internship</h3>
              <span class="qualification__subtitle">
                Master's degree - University of Deakin, Australia
              </span>
              <div class="qualification__calendar">
                <i class="far fa-calendar"></i> 2020
              </div>
            </div>

            <div>
              <span class="qualification__rounded"> </span>
              <span class="qualification__line"> </span>
            </div>
          </div>
          <div class="qualification__data">
            <div></div>
            <div>
              <span class="qualification__rounded"> </span>
              <span class="qualification__line"> </span>
            </div>
            <div>
              <h3 class="qualification__title">External Internship</h3>
              <span class="qualification__subtitle"> Moudjib Digital </span>
              <div class="qualification__calendar">
                <i class="far fa-calendar"></i> 2019
              </div>
            </div>
          </div>
          <div class="qualification__data">
            <div>
              <h3 class="qualification__title">End-Of-Degree internship</h3>
              <span class="qualification__subtitle">
                Bachelor's degree - Algeria Post
              </span>
              <div class="qualification__calendar">
                <i class="far fa-calendar"></i> 2018
              </div>
            </div>

            <div>
              <span class="qualification__rounded"> </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>


<script>
export default {
  name: "Qualification",
  components: {},
  data() {
    return {
      showEducation: false,
      showWork: true,
      showInternship: false,
    };
  },
  methods: {
    showEducationFunction: function () {
      this.showEducation = true;
      this.showWork = false;
      this.showInternship = false;
    },
    showWorkFunction: function () {
      this.showEducation = false;
      this.showWork = true;
      this.showInternship = false;
    },
    showInternshipFunction: function () {
      this.showEducation = false;
      this.showWork = false;
      this.showInternship = true;
    },
  },
};
</script>