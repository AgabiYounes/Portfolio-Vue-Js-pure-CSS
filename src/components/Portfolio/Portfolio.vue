<template>
  <section class="portfolio section" id="portfolio">
    <h2 class="section__title">Portfolio</h2>
    <span class="section__subtitle"> Most recent work </span>
    <div class="portfolio__container container swiper-container">
      <div class="swiper-wrapper">
        <Swiper :portfolio="youtaqa"></Swiper>
        <Swiper :portfolio="idnap"></Swiper>
        <Swiper :portfolio="adexcloud"></Swiper>
        <Swiper :portfolio="adextechnology"></Swiper>
        <Swiper :portfolio="adextraining"></Swiper>
        <Swiper :portfolio="efrevent"></Swiper>
      </div>
    </div>
  </section>
</template>


<script>
import Swiper from "./Swiper";
export default {
  name: "Portfolio",
  components: {
    Swiper,
  },
  data() {
    return {
      youtaqa: {
        portfolio__title: "YouTaQA",
        portfolio__description:
          "YouTaQA is a powerful Q&A system that provides a complete pipeline. Unlike existing QA systems, our system allows users to have accurate answers to their questions based entirely on our search engine.",
        portfolio__img: "youtaqa.png",
        portfolio__url: "https://github.com/AgabiYounes/YouTaQA",
      },
      idnap: {
        portfolio__title: "IDNAP",
        portfolio__description:
          "IDNAP (Numeric Identifier Algeria Post) is a responsive web application based on the MVC architecture which allows to manage the digital identifiers of Algerie Poste's customers.",
        portfolio__img: "idnap.png",
        portfolio__url: "https://github.com/AgabiYounes/IDNAP",
      },
      adexcloud: {
        portfolio__title: "ADEX Cloud",
        portfolio__description:
          "A web platform for the online purchase of ADEX Cloud products with SATIM E-Payment.",
        portfolio__img: "adexcloud.png",
        portfolio__url: "https://adexcloud.dz/",
      },
      adextechnology: {
        portfolio__title: "ADEX Technology",
        portfolio__description:
          "A Web site for the integration/Cloud company ADEX Technology.",
        portfolio__img: "adextechnology.png",
        portfolio__url: "https://www.adextechnology.dz/",
      },
      adextraining: {
        portfolio__title: "ADEX Training",
        portfolio__description: "Web platform for the ADEX Training Center.",
        portfolio__img: "adextraining.png",
        portfolio__url: "https://www.adextraining.dz/",
      },
      efrevent: {
        portfolio__title: "Efrevent",
        portfolio__description:
          "Implementation of an event-driven web platform based on a RESTFul API.",
        portfolio__img: "efrevent.png",
        portfolio__url: "http://efrevent.com/",
      },
    };
  },
  methods: {},
};
</script>
