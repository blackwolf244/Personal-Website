<script></script>

<template>
  <h1>Projects I'm working on</h1>
  <p>I dabbled in multiple areas but seems like I mostly fell in love with web development.
  </p>
  <p>Feel free to check my GitHub, CodePen and Projects i'm involved in!</p>


  <div class="spacing cnt wrapped">
    <div data-tooltip="In progress">
      <span class="project inprogress linkEffect">
        Blog<i class="ri-hammer-line"></i>
      </span>
    </div>
    <div data-tooltip="In progress">
      <span class="project inprogress linkEffect">
        Obsidian-TF-IDF-Tagger<i class="ri-hammer-line"></i>
      </span>
    </div>
  </div>

  <div class="cnt spacing">
    <span class="project linkEffect"><a href="https://webxr-library.web.app/">WebXR Library</a></span>
    <span class="project linkEffect"><a href="https://github.com/blackwolf244/tabliss-dark-glass">Tabliss Dark
        Glass</a></span>
    <span class="project linkEffect"><a href="https://enerplanet.th-deg.de/">EnerPlanET-Web-App</a></span>
  </div>

  <div class="spacing social-container">
    <div class="social-icons">
      <a target="_blank" rel="noopener noreferrer" class="social-icon" data-tooltip="GitHub"
        href="https://github.com/blackwolf244"><span class="sr">GitHub</span><i class="ri-github-line"></i></a>
      <a target="_blank" rel="noopener noreferrer" class="social-icon" data-tooltip="CodePen"
        href="https://codepen.io/blackwolf244"><span class="sr">CodePen</span><i class="ri-codepen-line"></i></a>
    </div>
    <!-- <div class="social-icons">
      <a target="_blank" rel="noopener noreferrer" class="social-icon" data-tooltip="WebXRLibrary"
        href="https://webxr-library.web.app/"><span class="sr">WebXR Library</span><i class="ri-stack-fill"></i></a>
    </div> -->
  </div>
</template>

<style scoped>
h1 {
  text-transform: uppercase;
  padding-bottom: 3rem;
  letter-spacing: 2px;
}

.linkEffect,
.linkEffect * {
  font-weight: 400;
}



h2 {
  padding-bottom: 1.5rem;
}

p {
  letter-spacing: 1.5px;
  line-height: 24px;
  padding-bottom: 1rem;
}

.cnt {
  width: 80%;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.wrapped {
  display: flex;
  width: fit-content;
}

.spacing {
  margin-top: 10px;
}

.project {
  flex-wrap: nowrap;
  text-wrap: nowrap;
  padding: 4px;
  text-decoration: none;
  display: flex;
  letter-spacing: 2px;
}

.inprogress:hover {
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

.inprogress i {
  transform: rotate(20deg);
}

.social-icons {
  float: left;
  display: flex;
  padding-top: 1rem;
  padding-bottom: 2rem;
  justify-content: space-between;
  margin-right: 0.5rem;
}

.social-icons~.social-icons {
  margin-right: 0;
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
  font-size: 1.5rem;
  text-decoration: none;
  margin-right: clamp(5px, 5vw, 2.5rem);
}

.social-icon:hover {
  border: solid 2px;
}

@media only screen and (min-width: 768px) {

  /* For desktop: */
  .social-icons {
    float: left;
    display: flex;
    padding-top: 1rem;
    padding-bottom: 2rem;
    justify-content: space-between;
    margin-right: 3rem;
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
    margin-right: clamp(10px, 5vw, 2.5rem);
  }
}
</style>