<template>
  <div class="blur">
    <div id="blob"></div>
  </div>
</template>

<script>
export default {
  mounted() {
    /* -- Glow effect -- */
    const blob = document.getElementById("blob");
    let animationFrameId = null;

    window.onpointermove = event => {
      const { clientX, clientY } = event;

      animationFrameId = requestAnimationFrame(() => {
        blob.animate({
          left: `${clientX}px`,
          top: `${clientY}px`
        }, { duration: 5000, fill: "forwards" });
      });
    }
  },
}

</script>

<style scoped>
#blob {
  height: 34vmax;
  aspect-ratio: 1;
  position: absolute;
  left: 50%;
  top: 50%;
  translate: -50% -50%;
  border-radius: 50%;
  background: linear-gradient(to right, var(--q), var(--p));
  animation: spin 10s linear infinite;
  opacity: 0.5;
}

@keyframes spin {

  100% {
    transform: rotate(360deg);
  }
}

.blur {
  pointer-events: none;
  z-index: 2;
  filter: blur(5vmax) brightness(80%) opacity(50%);
}

@media (prefers-reduced-motion) {
  .blur {
    display: none;
  }
}
</style>