<script setup lang="ts">

import MyTechnology from "./UI/MyTechnology.vue";

interface Technology {
  title: string,
  image: string,
}

const technologies: Array<Technology> = [
  {
    title: "HTML",
    image: "/technologies/HTML.svg",
  },
  {
    title: "CSS",
    image: "/technologies/CSS.svg",
  },
  {
    title: "JavaScript",
    image: "/technologies/JAVASCRIPT.svg",
  },
  {
    title: "TypeScript",
    image: "/technologies/TYPESCRIPT.svg",
  },
  {
    title: "Vue",
    image: "/technologies/VUE.svg",
  },
  {
    title: "React",
    image: "/technologies/REACT.svg",
  },
  {
    title: "Node.JS",
    image: "/technologies/NODE.svg",
  },
  {
    title: "Git",
    image: "/technologies/GIT.svg",
  },
  {
    title: "Tailwind",
    image: "/technologies/TAILWIND.svg",
  },
  {
    title: "SCSS",
    image: "/technologies/SCSS.svg",
  }
];

</script>

<template>
  <section class="main_component">
    <div class="main_text">
      <h1>
        Hi there, I'm <code> Moloдец</code>
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
  gap: clamp(40px, 2.5vw, 120px);
  width: 100%;
  & .me {
    margin-top: clamp(0px, 3vw, 50px);
    width: clamp(150px, 25vw, 400px);
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
  font-size: clamp(20px, 3vw, 60px);
  font-family: Poppins, sans-serif;
  color: white;
  & code {
    font-size: clamp(20px, 3vw, 60px);
  }
}
h3 {
  display: flex;
  justify-content: center;
  font-size: clamp(4px, 1.2vw, 1.5rem);
  font-family: Poppins, sans-serif;
  border: 1px solid wheat;
  background-color: wheat;
  border-radius: clamp(2px, 1vw, 10px);
  width: 300px;
  height: clamp(20px, 3vw, 60px);
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
  font-size: clamp(10px, 2vw, 20px);
  font-family: Poppins, sans-serif;
}
h6 {
  color: white;
  font-size: 20px;
  font-family: Poppins, sans-serif;
}
.blocks {
  display: flex;
  gap: clamp(6px, 1vw, 20px);
  flex-wrap: wrap;
  width: clamp(32vw, 60vw, 30vw);
}


</style>