<template>
  <div id="app">
    <notifications/>
    <Header></Header>
    <main class="main">
      <Home></Home>
      <About></About>
      <Skills></Skills>
      <Qualification></Qualification>
      <Portfolio></Portfolio>
      <Project></Project>
      <Testimonial></Testimonial>
      <Contact></Contact>
    </main>
    <Footer></Footer>
    <ScrollUpButton></ScrollUpButton>
  </div>
</template>

<script>
import Header from "@/components/Header/Header.vue";
import Home from "@/components/Home/Home.vue";
import About from "@/components/About/About.vue";
import Skills from "@/components/Skills/Skills.vue";
import Qualification from "@/components/Qualification/Qualification.vue";
import Portfolio from "@/components/Portfolio/Portfolio.vue";
import Project from "@/components/Project/Project.vue";
import Testimonial from "@/components/Testimonial/Testimonial.vue";
import Contact from "@/components/Contact/Contact.vue";
import Footer from "@/components/Footer/Footer.vue";
import ScrollUpButton from "@/components/ScrollUpButton/ScrollUpButton.vue";

export default {
  name: "App",
  components: {
    Header,
    Home,
    About,
    Skills,
    Qualification,
    Portfolio,
    Project,
    Testimonial,
    Contact,
    Footer,
    ScrollUpButton,
  },
};
</script>
