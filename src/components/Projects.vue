<script></script>

<template>
  <h1>Projects I'm working on</h1>
  <p>To keep on learning you have to keep on trying new stuff so I do!</p>
  <p>Check out some of my Projects on GitHub and Dribbble!</p>
  <div class="social-icons">
    <a
      target="_blank"
      rel="noopener noreferrer"
      class="social-icon"
      href="https://dribbble.com/StKern"
      data-tooltip="Dribble"
      ><span class="sr">Dribble</span><i class="ri-dribbble-line"></i
    ></a>
    <a
      target="_blank"
      rel="noopener noreferrer"
      class="social-icon"
      data-tooltip="Github"
      href="https://github.com/blackwolf244"
      ><span class="sr">GitHub</span><i class="ri-github-line"></i
    ></a>
  </div>
  <h2>Check out my Blog:</h2>
  <div class="cnt">
    <div class="blog">
      <p>Still in Development</p>
      <i class="ri-hammer-line"></i>
    </div>
  </div>
</template>

<style scoped>
h1 {
  text-transform: uppercase;
  padding-bottom: 3rem;
  letter-spacing: 2px;
}

h2 {
  padding-bottom: 1.5rem;
}

p {
  font-size: 1rem;
  letter-spacing: 1.5px;
  line-height: 24px;
  padding-bottom: 0.6rem;
}

.blog {
  text-decoration: none;
  padding: 10px;
  width: 200px;
  max-width: 600px;
  display: flex;
  align-items: center;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--text);
  border: 1px dashed;
  border-color: var(--border);
  border-radius: 5px;
}

.blog:hover {
  animation: shake 0.82s cubic-bezier(0.36, 0.07, 0.19, 0.97) both;
  transform: translate3d(0, 0, 0);
  backface-visibility: hidden;
  perspective: 1000px;
}

@keyframes shake {
  10%,
  90% {
    transform: translate3d(-1px, 0, 0);
  }

  20%,
  80% {
    transform: translate3d(2px, 0, 0);
  }

  30%,
  50%,
  70% {
    transform: translate3d(-4px, 0, 0);
  }

  40%,
  60% {
    transform: translate3d(4px, 0, 0);
  }
}

.blog p {
  padding-bottom: 0;
  line-height: 28px;
}

.blog i {
  position: relative;
  font-size: 1.5rem;
  padding-left: 25px;
  transform: rotate(20deg);
  bottom: 5px;
}

.social-icons {
  min-width: 100px;
  max-width: 150px;
  display: flex;
  padding-top: 1rem;
  padding-bottom: 2rem;
  justify-content: space-between;
}
.social-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--text);
  border: solid 1px;
  border-color: var(--border);
  width: 50px;
  height: 50px;
  border-radius: 50%;
  cursor: pointer;
  font-family: "Helvetica Neue", "Helvetica", "Arial", sans-serif;
  font-size: 2rem;
  text-decoration: none;
}

.social-icon:hover {
  border: solid 2px;
}

@media only screen and (min-width: 1200px) {
  /* For desktop: */
}
</style>