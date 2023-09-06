<template>
  <h1>Public Assets</h1>
  <p>Templates, Designs and Documents based upon my own research,
  </p>
  <p>for everyone and free to use.</p>
  <div>
    <div class="social-icons">
      <a target="_blank" rel="noopener noreferrer" class="social-icon" data-tooltip="GitHub"
        href="https://github.com/blackwolf244"><span class="sr">GitHub</span><i class="ri-github-line"></i></a>
      <a target="_blank" rel="noopener noreferrer" class="social-icon" data-tooltip="CodePen"
        href="https://codepen.io/blackwolf244"><span class="sr">CodePen</span><i class="ri-codepen-line"></i></a>
    </div>
    <div class="social-icons">
      <a target="_blank" rel="noopener noreferrer" class="social-icon" data-tooltip="WebXRLibrary"
        href="https://webxr-library.web.app/"><span class="sr">WebXR Library</span><i class="ri-stack-fill"></i></a>
      <a target="_blank" rel="noopener noreferrer" class="social-icon" data-tooltip="Pebblebox"
        href="https://github.com/blackwolf244/Ionic-Pebblebox"><span class="sr">PebbleBox</span><i
          class="ri-code-s-slash-line"></i></a>
    </div>

  </div>
  <h2>Tools:</h2>
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
  padding-bottom: 1rem;
}

.blog {
  text-decoration: none;
  padding: 10px;
  width: 200px;
  height: 70px;
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

.social-icon:hover {
  border: solid 2px;
}

@media only screen and (min-width: 1200px) {
  /* For desktop: */
}
</style>