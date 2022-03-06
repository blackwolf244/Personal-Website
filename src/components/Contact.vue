<script></script>

<template>
  <h1>Hey!</h1>
  <p>Feel free to get in touch via Email or LinkedIn!</p>
  <p>I'd love to hear more about you or your Ideas!</p>
  <h1>Let's have a chat!</h1>
  <p>
    Office times: <br />
    Mon - Fri // 11am - 5pm (GMT+1)
  </p>
  <div class="swrap">
    <div class="social-icons">
      <a
        target="_blank"
        aria-label="Email"
        rel="noopener noreferrer"
        class="social-icon"
        href="mailto:stefan.kern@protonmail.com"
        data-tooltip="stefan.kern@protonmail.com"
        ><span class="sr">stefan.kern@protonmai.com</span
        ><i class="ri-mail-add-line"></i
      ></a>
      <a
        target="_blank"
        aria-label="LinkedIn"
        rel="noopener noreferrer"
        class="social-icon"
        href="https://www.linkedin.com/in/stefan-kern-817791201"
        data-tooltip="LinkedIn"
        ><span class="sr">LinkedIn</span><i class="ri-linkedin-line"></i
      ></a>
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
  text-transform: uppercase;
  padding-bottom: 1rem;
  padding-top: 2rem;
  letter-spacing: 2px;
}

p {
  letter-spacing: 1.5px;
  line-height: 24px;
  padding-bottom: 1.5rem;
}
el {
  padding-bottom: 0;
}
.social-icons {
  min-width: 100px;
  max-width: 150px;
  display: flex;
  padding-top: 1rem;
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
  border-color: var(--border);
}

@media only screen and (min-width: 768px) {
  /* For desktop: */
}
</style>