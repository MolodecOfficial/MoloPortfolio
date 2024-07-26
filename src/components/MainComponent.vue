<script setup lang="ts">

import MyTechnology from "./UI/MyTechnology.vue";

interface Technology {
  title: string,
  image: string,
}

const technologies: Array<Technology> = [
  {
    title: "HTML",
    image: "src/assets/pics/technologies/HTML.png",
  },
  {
    title: "CSS",
    image: "src/assets/pics/technologies/CSS.png",
  },
  {
    title: "JavaScript",
    image: "src/assets/pics/technologies/JAVASCRIPT.png",
  },
  {
    title: "TypeScript",
    image: "src/assets/pics/technologies/TYPESCRIPT.png",
  },
  {
    title: "Vue",
    image: "src/assets/pics/technologies/VUE.png",
  },
  {
    title: "React",
    image: "src/assets/pics/technologies/REACT.png",
  },
  {
    title: "Node.JS",
    image: "src/assets/pics/technologies/NODE.png",
  },
  {
    title: "Git",
    image: "src/assets/pics/technologies/GIT.png",
  },
  {
    title: "Tailwind",
    image: "src/assets/pics/technologies/TAILWIND.png",
  },
  {
    title: "SCSS",
    image: "src/assets/pics/technologies/SCSS.png",
  }
];

</script>

<template>
  <section class="main_component">
    <div class="main_text">
      <h1>
        Hi there, I'm <code>Moloдец</code>
      </h1>
      <div class="jobs">
        <h3>
          Frontend Developer
        </h3>
        <h3>
          UI/UX Designer
        </h3>
      </div>
      <h5>
        Working since June 2023
      </h5>
      <section class="blocks">
        <MyTechnology
            v-for="(tech, idx) in technologies"
            :key="idx"
            :image="tech.image"
            :title="tech.title"
        />
      </section>
    </div>
      <img class="me" src="../../public/logo.jpg" alt="">
  </section>

</template>

<style scoped>
.main_component {
  margin-top: 150px;
  justify-content: center;
  align-items: center;
  display: flex;
  flex-direction: row;
  gap: 120px;
  width: 100%;
  & .me {
    margin-top: 50px;
    width: 400px;
    border-radius: 30px;
  }
}
.main_text {
  flex-direction: column;
  display: flex;
  row-gap: 15px;
  width: 30vw;
}
h1 {
  font-size: 50px;
  font-family: Poppins, sans-serif;
  color: white;
  & code {
    font-size: 60px;
  }
}
h3 {
  display: flex;
  justify-content: center;
  font-size: 24px;
  font-family: Poppins, sans-serif;
  border: 1px solid wheat;
  background-color: wheat;
  border-radius: 10px;
  width: 300px;
  height: 60px;
  align-items: center;
  color: black;
}
.jobs {
  display: flex;
  gap: 10px;
}
h5 {
  display: flex;
  justify-content: center;
  color: white;
  font-size: 20px;
  font-family: Poppins, sans-serif;
}
h6 {
  color: white;
  font-size: 20px;
  font-family: Poppins, sans-serif;
}
.blocks {
  display: flex;
  gap: 20px;
  flex-wrap: wrap;
  width: 30vw;
}


</style>