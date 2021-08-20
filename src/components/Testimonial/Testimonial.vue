<template>
  <section class="testimonial section">
    <h2 class="section__title">Testimonial</h2>
    <span class="section__subtitle">
      What my colleagues and superiors say about me
    </span>
    <div class="testimonial__container container swiper-container">
      <div class="swiper-wrapper">
        <TestimonialPeople
          :testimonial__person="testimonialAhmed"
        ></TestimonialPeople>
        <TestimonialPeople
          :testimonial__person="testimonialKatia"
        ></TestimonialPeople>
        <TestimonialPeople
          :testimonial__person="testimonialRahmani"
        ></TestimonialPeople>
        <TestimonialPeople
          :testimonial__person="testimonialAkram"
        ></TestimonialPeople>
        <TestimonialPeople
          :testimonial__person="testimonialRayane"
        ></TestimonialPeople>
        <TestimonialPeople
          :testimonial__person="testimonialSidAli"
        ></TestimonialPeople>
      </div>
    </div>
  </section>
</template>

<script>
import TestimonialPeople from "./TestimonialPeople.vue";
export default {
  components: { TestimonialPeople },
  name: "Testimonial",

  data() {
    return {
      testimonialAhmed: {
        testimonial__img: "ahmed.jpg",
        testimonial__name: "Ahmed DJOUDI",
        testimonial__client: "Co-worker",
        testimonial__description:
          "I'm very pleased to write down a brief recommendation about YOUNES AGABI. I have worked with Younes at ADEX TECHNOLOGY where I noticed his talent and skills in Frontend Developemnt and Web Design. YOUNES has a very big ambition to learn, evolve and master new technologies very fast. He is very cooperative with his work team and really helpful in transferring knowledge and experience to them.",
        testimonial__icon_star: 5,
      },
      testimonialKatia: {
        testimonial__img: "katia.jpg",
        testimonial__name: "Katia MOUFFOK",
        testimonial__client: "Co-worker",
        testimonial__description:
          "Rayane is a very focus and talented person, his work is fascinating. He consistently seeks out constructive feedback so that he improves his self, both personally and professionally. His qualities as a team member are outstanding, he communicates very well with other team members and successfully established flourishing relationships with other departments as well. I am certain that Rayane is going to continue to do creative work in his future.",
        testimonial__icon_star: 5,
      },
      testimonialAkram: {
        testimonial__img: "akram.jpg",
        testimonial__name: "Akram ARAR",
        testimonial__client: "Ex Co-worker",
        testimonial__description:
          "I studied and worked in the same company as Younes for a long time. Younes id always curious and open-minded, he has a real taste for challenges! He is always willing to answer various questions and to think of solutions to the most complex problems. New responsibilities and management do not scare him: although effective alone, he has a sense of teamwork and knows how to motivate teams when a project is entrusted to him.",
        testimonial__icon_star: 5,
      },
      testimonialRayane: {
        testimonial__img: "rayane.jpg",
        testimonial__name: "Rayan KRIMI",
        testimonial__client: "Ex Co-worker",
        testimonial__description:
          "Younes is a talented meticulous and creative young web developer who loves his work. With great potential and innovative ideas, He is a person who inspires unusual comfort when working with him and above all a person who does not do things by halves Good luck younes",
        testimonial__icon_star: 5,
      },
      testimonialSidAli: {
        testimonial__img: "SidAli.jpg",
        testimonial__name: "Sidali BOUTALEB",
        testimonial__client: "SidAli Managed Younes directly",
        testimonial__description:
          "Younes is a quality IT developer, motivated, responsible, likes teamwork.",
        testimonial__icon_star: 5,
      },
      testimonialRahmani: {
        testimonial__img: "Rahmani.jpg",
        testimonial__name: "Amine Rahmani",
        testimonial__client: "Amine Was Younes's Teacher",
        testimonial__description:
          "Mr. AGABI is charismatic and creative, and thinks outside the box. He has demonstrated skills in acquiring and applying knowledge from his studies. Assiduous, curious and enthusiastic, he has always provided quality work through individual and group exercises.",
        testimonial__icon_star: 5,
      },
    };
  },
};
</script>