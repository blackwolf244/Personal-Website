<script>
</script>

<template>
  <footer>
    <div class="remix">
      <a target="_blank" rel="noopener noreferrer" class="social-icon" data-tooltip="Icons by Remix Icons"
        href="https://remixicon.com/">
        <div class="socialicon">
          <span class="sr">Remix Icons</span><i class="ri-remixicon-line"></i>
        </div>
        <div class="rlabel">
          <p>Remix Icons</p>
        </div>
      </a>
    </div>
  </footer>
</template>

<style scoped>
footer {
  position: absolute;
  left: 0;
  bottom: 0;
  width: 100%;
  height: 75px;
  padding-right: 2.5rem;
  padding-left: 4rem;
}

.remix {
  height: 1rem;
  width: fit-content;
  display: flex;
  float: right;
  padding-bottom: 40px;
}

.remix a {
  width: fit-content;
}

.rlabel {
  display: flex;
  float: left;
  align-items: center;
}

.rlabel p {
  text-transform: uppercase;
  max-width: 100%;
  font-size: small;
}

.social-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--text);
  width: 35px;
  height: 35px;
  cursor: pointer;
  font-family: "Helvetica Neue", "Helvetica", "Arial", sans-serif;
  font-size: 1.2rem;
  text-decoration: none;
}

.social-icon:hover {
  border-bottom: solid 2px;
}

@media only screen and (min-width: 768px) {

  /* For desktop: */
  footer {
    padding-left: 10rem;
  }
}

@media only screen and (min-width: 1200px) {

  /* For desktop: */
  footer {
    padding-left: 15rem;
  }
}
</style>