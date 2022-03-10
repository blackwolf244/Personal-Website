<script setup>
import Landing from "./components/Landing.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";
import Nav from "./components/Nav.vue";
import { createDOMCompilerError } from "@vue/compiler-dom";
</script>

<template>
  <div>
    <Nav></Nav>
    <div class="container">
      <section id="landing">
        <Landing />
      </section>

      <section id="projects">
        <Projects />
      </section>

      <section id="contact">
        <Contact />
      </section>
    </div>
  </div>

  <!-- <HelloWorld msg="Hello Vue 3 + Vite" /> -->
</template>

<style>
:root {
  --pdark: #ff5303;
  --plight: #562ef2;
  --color-white: #fff;
  --color-black: #000;
}

.light {
  --bg: var(--color-white);
  --p: var(--plight);
  --text: var(--color-black);
  --border: var(--color-black);
}

.dark {
  --bg: var(--color-black);
  --p: var(--pdark);
  --text: var(--color-white);
  --border: var(--color-white);
}

/* .light {
  background-color: 
} */

* {
  margin: 0px;
  padding: 0;
  box-sizing: border-box;
}

body {
  background-color: var(--bg);
}

h1 {
  color: var(--text);
}

h2 {
  color: var(--text);
  text-transform: uppercase;
  font-weight: normal;
  font-size: 1.2rem;
}

p {
  color: var(--text);
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
section {
  padding-top: 40px;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding-right: 3rem;
  padding-left: 2.3rem;
  scroll-snap-align: start;
}

.container {
  scroll-snap-type: y mandatory;
  overflow-y: scroll;
  height: 100vh;
}

[data-tooltip] {
  position: relative;
  z-index: 10;
}

/* Positioning and visibility settings of the tooltip */
[data-tooltip]:before,
[data-tooltip]:after {
  position: absolute;
  visibility: hidden;
  opacity: 0;
  left: 50%;
  bottom: calc(100% + 5px); /* 5px is the size of the arrow */
  pointer-events: none;
  transition: 0.1s;
  will-change: transform;
}

/* The actual tooltip with a dynamic width */
[data-tooltip]:before {
  content: attr(data-tooltip);
  padding: 10px;
  min-width: 50px;
  max-width: 250px;
  width: max-content;
  width: -moz-max-content;
  border-radius: 6px;
  font-size: 14px;
  font-weight: normal;
  background-color: var(--bg);
  border: 1px solid;
  border-color: var(--border);
  color: var(--text);
  text-align: center;
  word-wrap: break-word;
  white-space: pre-wrap;
  transform: translate(-50%, -5px) scale(0.5);
}

/* Tooltip arrow */
[data-tooltip]:after {
  content: "";
  border-style: solid;
  border-width: 5px 5px 0px 5px; /* CSS triangle */
  border-color: var(--border) transparent transparent transparent;
  transition-duration: 0s; /* If the mouse leaves the element, 
                              the transition effects for the 
                              tooltip arrow are "turned off" */
  transform-origin: top; /* Orientation setting for the
                              slide-down effect */
  transform: translateX(-50%) scaleY(0);
}

/* Tooltip becomes visible at hover */
[data-tooltip]:hover:before,
[data-tooltip]:hover:after {
  visibility: visible;
  opacity: 1;
}
/* Scales from 0.5 to 1 -> grow effect */
[data-tooltip]:hover:before {
  transition-delay: 0.2s;
  transform: translate(-50%, -5px) scale(1);
}
/* 
  Arrow slide down effect only on mouseenter (NOT on mouseleave)
*/
[data-tooltip]:hover:after {
  transition-delay: 0.2s; /* Starting after the grow effect */
  transition-duration: 0.2s;
  transform: translateX(-50%) scaleY(1);
}
/*
  That's it for the basic tooltip.

  If you want some adjustability
  here are some orientation settings you can use:
*/

/* LEFT */
/* Tooltip + arrow */
[data-tooltip-location="left"]:before,
[data-tooltip-location="left"]:after {
  left: auto;
  right: calc(100% + 5px);
  bottom: 50%;
}

/* Tooltip */
[data-tooltip-location="left"]:before {
  transform: translate(-5px, 50%) scale(0.5);
}
[data-tooltip-location="left"]:hover:before {
  transform: translate(-5px, 50%) scale(1);
}

/* Arrow */
[data-tooltip-location="left"]:after {
  border-width: 5px 0px 5px 5px;
  border-color: transparent transparent transparent var(--border);
  transform-origin: left;
  transform: translateY(50%) scaleX(0);
}
[data-tooltip-location="left"]:hover:after {
  transform: translateY(50%) scaleX(1);
}

/* RIGHT */
[data-tooltip-location="right"]:before,
[data-tooltip-location="right"]:after {
  left: calc(100% + 5px);
  bottom: 50%;
}

[data-tooltip-location="right"]:before {
  transform: translate(5px, 50%) scale(0.5);
}
[data-tooltip-location="right"]:hover:before {
  transform: translate(5px, 50%) scale(1);
}

[data-tooltip-location="right"]:after {
  border-width: 5px 5px 5px 0px;
  border-color: transparent var(--border) transparent transparent;
  transform-origin: right;
  transform: translateY(50%) scaleX(0);
}
[data-tooltip-location="right"]:hover:after {
  transform: translateY(50%) scaleX(1);
}

/* BOTTOM */
[data-tooltip-location="bottom"]:before,
[data-tooltip-location="bottom"]:after {
  top: calc(100% + 5px);
  bottom: auto;
}

[data-tooltip-location="bottom"]:before {
  transform: translate(-50%, 5px) scale(0.5);
}
[data-tooltip-location="bottom"]:hover:before {
  transform: translate(-50%, 5px) scale(1);
}

[data-tooltip-location="bottom"]:after {
  border-width: 0px 5px 5px 5px;
  border-color: transparent transparent var(--border) transparent;
  transform-origin: bottom;
}

/* Utility class to hide content visually while keeping it screen reader-accessible.
 Source: https://www.scottohara.me/blog/2017/04/14/inclusively-hidden.html  */

.sr:not(:focus):not(:active) {
  clip: rect(0 0 0 0);
  clip-path: inset(100%);
  height: 1px;
  overflow: hidden;
  position: absolute;
  white-space: nowrap;
  width: 1px;
}

@media only screen and (min-width: 768px) {
  /* For desktop: */
  section {
    height: 100vh;
    padding-right: 3rem;
    padding-left: 10rem;
    padding-top: 50px;
    scroll-snap-align: start;
  }

  h1 {
    font-size: 2.4rem;
  }
  h2 {
    font-size: 1.5rem;
  }
  p {
    max-width: 70%;
  }
}

@media only screen and (min-width: 1200px) {
  /* For desktop: */
  section {
    height: 100vh;
    padding-right: 3rem;
    padding-left: 15rem;
    padding-top: 0px;
    scroll-snap-align: start;
  }

  h1 {
    font-size: 2.4rem;
  }
  h2 {
    font-size: 1.5rem;
  }
  p {
    max-width: 65%;
  }
}

@media (prefers-color-scheme: dark) {
  .light {
    --bg: var(--color-black);
    --p: var(--pdark);
    --text: var(--color-white);
    --border: var(--color-white);
  }
}
</style>
