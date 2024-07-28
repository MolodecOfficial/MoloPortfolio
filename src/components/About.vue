<script setup lang="ts" xmlns:color="http://www.w3.org/1999/xhtml">

</script>

<template>
  <section>
    <div class="container">
      <article class="header">
        <h1>&#8595;</h1><h2>About me</h2><h1>&#8595;</h1>
      </article>
      <section class="about-text">
        <article class="about-main-text">
          <p>
            I decided to focus on frontend development in 2022, where I mastered <b style="color: #ec5b02">HTML5</b>, <b style="color: #029aec">CSS3</b>, and <b style="color: #ecc502">JavaScript</b>.
          </p>
          <p>
            Over time, I became more confident in my skills and started working on real projects. I chose <b style="color: #17b203">Vue</b> as my primary framework and successfully completed several projects using it. Additionally, I gained experience with <b style="color: #02a6ec">React</b>, which allowed me to expand my technological stack and understand the differences between popular libraries and frameworks.
            Recently, I started actively using <b style="color: #0151ff">TypeScript</b> and <b style="color: #18e3e3">TailwindCSS</b>.
          </p>
          <p>
            My <a href="https://github.com/MolodecOfficial">GitHub</a> is open for review, where you can check out my projects and evaluate my skills. I am always striving for excellence and am open to new challenges and opportunities.
          </p>
        </article>
        <article>
          <img src="../../public/img.png" alt="">
        </article>
      </section>
      <section class="next-text">
        <p>
          This is followed by a presentation of projects in which I participated as the main developer or assistant
        </p>
      </section>
    </div>
  </section>
</template>

<style scoped>
section {
  width: 100%;
  display: flex;
  justify-content: center;
}
.container {
  display: flex;
  flex-direction: column;
  width: 60%;
  text-align: center;
  row-gap: 8vw;
}
.header {
  display: flex;
  justify-content: center;
  gap: 50px;
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
.about-text {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 20px;
  & .about-main-text {
    display: flex;
    flex-direction: column;
    gap: clamp(10px, 2.5vw, 40px);
  }
  & img {
    width: clamp(100px, 30vw, 450px);
  }
}
p {
  font-size: clamp(10px, 2.5vw, 22px);
  font-family: Poppins, sans-serif;
  letter-spacing: 1px;
  color: white;
  z-index: 1;
}
a {
  text-decoration: none;
  font-weight: bold;
  color: lightblue;
}

</style>