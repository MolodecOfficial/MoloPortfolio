<script setup lang="ts">

</script>

<template>
  <section>
    <a href="https://discord.gg/CpwM2R5g">
      <img src="../../public/links/discord.png" alt="">
    </a>
    <a href="https://vk.com/molodec_official">
      <img src="../../public/links/vk.png" alt="">
    </a>
    <a href="https://t.me/molodec_official">
      <img src="../../public/links/telegram.png" alt="">
    </a>
    <a href="https://github.com/MolodecOfficial">
      <img src="../../public/links/github.png" alt="">
    </a>
  </section>
</template>

<style scoped>
section {
  display: flex;
  position: absolute;
  flex-direction: column;
  top: 50%;
  transform: translate(0, -50%);
  z-index: 1;
  & img {
    width: clamp(10px, 3.5vw, 40px);;
    margin: 10px;
    transition: all 0.15s ease-in-out;
    &:hover {
      scale: 1.3;
    }
  }
}
@media screen and (max-width: 480px){
  section {
    display: none;
  }
}
</style>