<script setup lang="ts">

</script>

<template>
  <div class="contact-container">
    <article class="contact__header">
      <h1>&#8595;</h1><h2>Contact Me</h2><h1>&#8595;</h1>
    </article>
    <section class="contact__main">
      <h3>I mostly use social media to get in touch about work, so follow the links below to start collaborating</h3>
      <section>
        <a href="https://discord.gg/CpwM2R5g">
          <img src="../assets/pics/links/discord.png" alt="">
        </a>
        <a href="https://vk.com/molodec_official">
          <img src="../assets/pics/links/vk.png" alt="">
        </a>
        <a href="https://t.me/molodec_official">
          <img src="../assets/pics/links/telegram.png" alt="">
        </a>
        <a href="https://github.com/MolodecOfficial">
          <img src="../assets/pics/links/github.png" alt="">
        </a>
      </section>
    </section>
  </div>
</template>

<style scoped>
.contact-container {
  display: flex;
  width: 100%;
  justify-content: center;
  flex-direction: column;
  gap: 9vw;
}
.contact__header {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 50px;
  transform: translate(0, 160%);
}
h1 {
  font-size: 40px;
  color: wheat;
  animation: up-to-down 1s infinite;
}
@keyframes up-to-down {
  50% {
    transform: translate(0, 30%);
  }
}
h2 {
  display: flex;
  justify-content: center;
  font-size: 50px;
  font-family: Poppins, sans-serif;
  color: wheat;
  z-index: 1;
}
h3 {
  color: white;
}
.contact__main {
  gap: 40px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  font-family: Poppins, sans-serif;
  align-items: center;
}
img {
  width: 50px;
  transition: all 0.2s ease-in-out;
  &:hover {
    scale: 1.3;
  }
}
section {
  display: flex;
  gap: 30px;
}
</style>