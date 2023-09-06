<script></script>

<template>
  <div class="wrapper">
    <div class="p1">
      <h1>
        <a target="_blank" rel="noopener noreferrer" href="https://techterms.com/definition/internet_of_things"
          data-tooltip="techterms.com" data-tooltip-location="right">IOT</a> and <a target="_blank"
          rel="noopener noreferrer" href="https://dev.to/emmabostian/ux-engineering-3hem"
          data-tooltip="dev.to">UX-Engineering</a> Enthusiast with
        Passion
      </h1>
      <p> <i>I am an Interactive Systems Engineer striving to improve and develop my skills as a Developer, Product
          Designer and UX
          Researcher.</i>
      </p>
      <p class="el">
        My current interests are accessible development, modular system design and generative art, so you'll see some
        <a href="#projects">projects</a> about those topics soon.
      </p>
    </div>
    <!-- <div class="illustration">
      <svg
        aria-hidden="true"
        focusable="false"
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="322"
        height="469"
        viewBox="0 0 322 469"
      >
        <defs>
          <path
            id="path-1"
            fill-rule="evenodd"
            d="M43 30h79c7.17489532 0 13 5.82510468 13 13v79c0 7.17489532-5.82510468 13-13 13H43c-7.17489532 0-13-5.82510468-13-13V43c0-7.17489532 5.82510468-13 13-13z"
          />
          <mask
            id="mask-2"
            x="0"
            y="0"
            maskContentUnits="userSpaceOnUse"
            maskUnits="userSpaceOnUse"
          >
            <rect width="322" height="469" x="0" y="0" fill="white" />
            <use fill="black" xlink:href="#path-1" />
          </mask>
          <path
            id="path-3"
            fill-rule="evenodd"
            d="M261 261h28c7.17489532 0 13 5.82510468 13 13v28c0 7.17489532-5.82510468 13-13 13h-28c-7.17489532 0-13-5.82510468-13-13v-28c0-7.17489532 5.82510468-13 13-13z"
          />
          <mask
            id="mask-4"
            x="0"
            y="0"
            maskContentUnits="userSpaceOnUse"
            maskUnits="userSpaceOnUse"
          >
            <rect width="322" height="469" x="0" y="0" fill="white" />
            <use fill="black" xlink:href="#path-3" />
          </mask>
          <path
            id="path-5"
            fill-rule="evenodd"
            d="M127 426h7c7.17489532 0 13 5.82510468 13 13v7c0 7.17489532-5.82510468 13-13 13h-7c-7.17489532 0-13-5.82510468-13-13v-7c0-7.17489532 5.82510468-13 13-13z"
          />
          <mask
            id="mask-6"
            x="0"
            y="0"
            maskContentUnits="userSpaceOnUse"
            maskUnits="userSpaceOnUse"
          >
            <rect width="322" height="469" x="0" y="0" fill="white" />
            <use fill="black" xlink:href="#path-5" />
          </mask>
        </defs>
        <g>
          <use
            fill-opacity="0"
            stroke="currentColor"
            stroke-linecap="butt"
            stroke-linejoin="miter"
            stroke-width="60"
            mask="url(#mask-2)"
            xlink:href="#path-1"
          />
          <use
            fill-opacity="0"
            stroke="currentColor"
            stroke-linecap="butt"
            stroke-linejoin="miter"
            stroke-width="40"
            mask="url(#mask-4)"
            xlink:href="#path-3"
          />
          <use
            fill-opacity="0"
            stroke="currentColor"
            stroke-linecap="butt"
            stroke-linejoin="miter"
            stroke-width="20"
            mask="url(#mask-6)"
            xlink:href="#path-5"
          />
        </g>
      </svg>
    </div> -->
  </div>
</template>

<style scoped>
.wrapper {
  width: 100%;
  display: inline-block;
}

.p1 {
  float: left;
}

.illustration {
  float: left;
  display: none;
  align-items: center;
  width: 30%;
  height: 100%;
}

svg {
  color: var(--p);
  height: 400px;
  width: 70%;
}

h1 {
  text-transform: uppercase;
  padding-bottom: 3rem;
  letter-spacing: 2px;
}


p {
  letter-spacing: 1.5px;
  line-height: 24px;
  padding-bottom: 1rem;
}

.el {
  padding-bottom: 0;
}

a {
  text-decoration: none;
  color: var(--p);
}

@media only screen and (min-width: 768px) {

  /* For desktop: */
  /* .p1 {
    width: 100%;
  } */
}

@media only screen and (min-width: 1200px) {
  /* For desktop: */

  /* .p1 {
    width: 60%;
  } */

  h1 {
    font-size: 3.5rem;
    max-width: 90%;
    padding-bottom: 6rem;
  }

  p {
    padding-bottom: 4rem;
  }

  .illustration {
    left: 0px;
    width: 30%;
    bottom: 10px;
    display: flex;
  }
}
</style>