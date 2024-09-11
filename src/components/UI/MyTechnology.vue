<script setup lang="ts">

const propsTechnology = defineProps( {
  image: String,
  title: String
})

</script>

<template>
  <div class="block">
    <img class="block_img" :src="propsTechnology.image" alt="" />
    <code>{{ propsTechnology.title }}</code>
  </div>
</template>

<style scoped>
.block {
  width: clamp(48px, 5vw, 5.15vw);
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  row-gap: clamp(2px, 1vw, 16px);
  border-radius: clamp(1px, 0.5vw, 10px);
  & .block_img {
    margin-top: 10px;
    width: clamp(18px, 4vw, 60px);
  }
  & code {
    color: white;
    margin-bottom: 10px;
    font-size: clamp(8px, 0.8vw, 15px);
    cursor: default;
  }
}
& .block:nth-child(1) {
  filter: drop-shadow(0 4px 2px #fa5b06);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #fa5b06);
  }
}
& .block:nth-child(2) {
  filter: drop-shadow(0 4px 2px #06b9fa);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #06b9fa);
  }
}
& .block:nth-child(3) {
  filter: drop-shadow(0 4px 2px #fad106);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #fad106);
  }
}
& .block:nth-child(4) {
  filter: drop-shadow(0 4px 2px #0680fa);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #0680fa);
  }
}
& .block:nth-child(5) {
  filter: drop-shadow(0 4px 2px #02b713);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #02b713);
  }
}
& .block:nth-child(6) {
  filter: drop-shadow(0 4px 2px #00da81);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #00da81);
  }
}
& .block:nth-child(7) {
  filter: drop-shadow(0 4px 2px #5bc505);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #5bc505);
  }
}
& .block:nth-child(8) {
  filter: drop-shadow(0 4px 2px #f36801);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #f36801);
  }
}
& .block:nth-child(9) {
  filter: drop-shadow(0 4px 2px #05c5af);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #05c5af);
  }
}
& .block:nth-child(10) {
  filter: drop-shadow(0 4px 2px #e340c1);
  transition: all 0.3s ease-in-out;
  &:hover {
    scale: 1.1;
    filter: drop-shadow(0 8px 4px #e340c1);
  }
}
</style>