<script setup lang="ts">
import Nav from "./components/Nav.vue";
import Links from "./components/Links.vue";
import MainComponent from "./components/MainComponent.vue";
import About from "./components/About.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <section class="home">
    <Nav/>
    <Links/>
    <MainComponent/>
  </section>
  <section>
    <About/>
  </section>
  <section>
    <Projects/>
  </section>
  <section>
    <Contact/>
  </section>
  <section>
    <Footer/>
  </section>
</template>

<style scoped>
.home {
  height: 100vh;
}
</style>
