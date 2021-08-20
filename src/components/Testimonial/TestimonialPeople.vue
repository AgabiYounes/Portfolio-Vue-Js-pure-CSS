<template>
  <div class="testimonial__content swiper-slide">
    <div class="testimonial__data">
      <div class="testimonial__header">
        <img
          :src="require(`@/assets/img/${testimonial__person.testimonial__img}`)"
          alt=""
          class="testimonial__img"
        />
        <div>
          <h3 class="testimonial__name">
            {{ testimonial__person.testimonial__name }}
          </h3>
          <span class="testimonial__client">{{
            testimonial__person.testimonial__client
          }}</span>
        </div>
      </div>
      <div>
        <i
          class="fas fa-star testimonial__icon-star"
          v-for="star in testimonial__person.testimonial__icon_star"
          :key="star"
        ></i>
      </div>
    </div>
    <p class="testimonial__description">
      {{ testimonial__person.testimonial__description }}
    </p>
  </div>
</template>

<script>
export default {
  name: "TestimonialPeople",

  data() {
    return {};
  },
  props: ["testimonial__person"],
};
</script>