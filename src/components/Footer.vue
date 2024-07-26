<script setup lang="ts">

</script>

<template>
  <section class="footer">
    <div class="footer_logo">
      <code>Molodec_Official 😺</code>
    </div>
    <section class="footer_menu">
      <a href="https://github.com/MolodecOfficial">GitHub</a>
      <a href="https://discord.gg/CpwM2R5g">Discord</a>
      <a href="https://t.me/molodec_official">Telegram</a>
      <a href="https://vk.com/molodec_official">VK</a>
    </section>
  </section>
</template>

<style scoped>
.footer {
  margin-top: 30px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.footer_logo {
  cursor: default;
  margin-left: 40px;
  color: rgba(142, 142, 142, 0.58);
  font-size: 25px;
  transition: all 0.1s ease-in-out;
  &:hover {
    color: wheat;
  }
}
.footer_menu {
  gap: 45px;
  margin-right: 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 40px;
  &.footer_menu a {
    font-family: Poppins, sans-serif;
    color: rgba(142, 142, 142, 0.58);
    text-decoration: none;
    font-size: 25px;
    transition: all 0.2s ease-in-out;
    &:hover {
      color: wheat;
    }
  }
}

</style>