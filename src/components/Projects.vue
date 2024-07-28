<script setup lang="ts">

import MyProjects from "./UI/MyProject.vue";

interface Project {
  image: string,
  name: string,
  link: string,
  code: string
}

const projects: Array<Project> = [
  {
    image: "/projects/bmpland.png",
    name: "BMPLand",
    link: "https://bmplandweb.vercel.app/",
    code: "https://github.com/MolodecOfficial/BMPLand"
  },
  {
    image: "/projects/canvas.png",
    name: "Canvas",
    link: "https://canvas-livid-nine.vercel.app/",
    code: "https://github.com/MolodecOfficial/Canvas"
  },
  {
    image: "/projects/k-telecom.png",
    name: "K-Telecom",
    link: "https://telecom-seven.vercel.app/",
    code: "https://github.com/MolodecOfficial/K-Telecom"
  },
  {
    image: "/projects/organizations.png",
    name: "Counting-Workers",
    link: "https://counting-workers.vercel.app/",
    code: "https://github.com/MolodecOfficial/Counting-Workers"
  },
  {
    image: "/projects/registerform.png",
    name: "RegisterForm",
    link: "https://github.com/MolodecOfficial",
    code: "https://github.com/MolodecOfficial/RegisterForm"
  },
  {
    image: "/projects/authors.png",
    name: "Authors-LGame",
    link: "https://github.com/MolodecOfficial",
    code: "https://github.com/MolodecOfficial/Authors"
  },
];
</script>

<template>
  <div class="projects-container">
    <article class="projects-header">
      <h1>&#8595;</h1><h2>Projects</h2><h1>&#8595;</h1>
    </article>
    <section class="projects-section">
      <MyProjects v-for="(proj, idx) in projects"
                :key="idx"
                :image="proj.image"
                :name="proj.name"
                :link="proj.link"
                :code="proj.code"
      />
    </section>
  </div>
</template>

<style scoped>
.projects-container {
  display: flex;
  flex-direction: column;
  gap: 13vw;
  width: 100%;
  justify-content: center;
  align-items: center;
}
.projects-header {
  display: flex;
  justify-content: center;
  gap: 50px;
  transform: translate(0, 160%);
}
.projects-section {
  display: flex;
  justify-content: center;
  gap: 40px;
  flex-wrap: wrap;
  width: 80%;
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
</style>