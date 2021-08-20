<template>
  <nav class="nav container">
    <a href="#" class="nav__logo">Younes AGABI</a>
    <div class="nav__menu" id="nav-menu" :class="{ show__menu: showMenu }">
      <ul class="nav__list grid">
        <li class="nav__item">
          <a href="#home" class="nav__link" @click="showMenu = false"
            ><i class="fas fa-home nav__icon"></i> Home</a
          >
        </li>
        <li class="nav__item">
          <a href="#about" class="nav__link" @click="showMenu = false"
            ><i class="fas fa-id-card nav__icon"></i> About</a
          >
        </li>
        <li class="nav__item">
          <a href="#skills" class="nav__link" @click="showMenu = false">
            <i class="fas fa-head-side-virus nav__icon"></i> Skills</a
          >
        </li>
        <li class="nav__item">
          <a href="#qualification" class="nav__link" @click="showMenu = false"
            ><i class="fas fa-briefcase nav__icon"></i> Experience</a
          >
        </li>
        <li class="nav__item">
          <a href="#portfolio" class="nav__link" @click="showMenu = false"
            ><i class="fas fa-images nav__icon"></i> Portfolio</a
          >
        </li>
        <li class="nav__item">
          <a href="#contact" class="nav__link" @click="showMenu = false"
            ><i class="fas fa-envelope nav__icon"></i> Contact</a
          >
        </li>
      </ul>
      <button class="nav__close" id="nav-close " @click="showMenu = !showMenu">
        <i class="fas fa-times"></i>
      </button>
    </div>
    <div class="nav__btns">
      <div>
        <button
          class="nav__toggle"
          id="nav-toggle "
          @click="showMenu = !showMenu"
          v-show="!showMenu"
        >
          <i class="fas fa-bars"></i>
        </button>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBar",

  data() {
    return {
      showMenu: false,
    };
  },
};
</script>