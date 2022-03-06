<script>
</script>

<template>
  <div class="topbar">
    <div class="focus">
      <a class="contact" href="#contact">Say Hi!</a>
      <a @click="increment" class="switch" href="#"
        ><span class="sr">Theme Switch</span><i class="ri-fire-line"></i
      ></a>
    </div>
  </div>
  <div class="sidebar">
    <div class="line">
      <h2>Kern <br />Stefan</h2>

      <i class="ri-arrow-down-s-line"></i>
    </div>
  </div>
</template>

<style scoped>
.topbar {
  position: fixed;
  display: block;
  top: 0;
  left: 0;
  padding-top: 20px;
  width: 100vw;
  height: 120px;
}
.sidebar {
  position: fixed;
  top: 0;
  left: 0;
  margin-top: 40px;
  margin-left: 1.4rem;
  height: calc(100vh - 80px);
  border-left: 1px solid;
  border-color: var(--border);
}
.sidebar h2 {
  padding-top: 5px;
  padding-left: 0.5rem;
  font-weight: normal;
  font-size: 1.2rem;
  text-transform: uppercase;
  text-orientation: mixed;
  writing-mode: vertical-rl;
}

.line {
  display: flex;
}

.line i {
  position: absolute;
  bottom: 0;
  font-size: 2rem;
  padding-left: 0.2rem;
  color: var(--text);
}

.focus {
  float: right;
  margin: 25px;
  margin-right: 30px;
  display: flex;
}

.contact {
  text-decoration: none;
  line-height: 23px;
  padding: 10px;
  font-weight: bold;
  font-size: 1rem;
  padding-left: 1.2rem;
  padding-right: 1.2rem;
  letter-spacing: 2px;
  text-transform: uppercase;
  text-align: center;
  color: var(--text);
  border: 2px solid;
  border-color: var(--border);
  border-radius: 5px;
}
.contact:hover {
  border: solid 3px;
}
.switch {
  display: flex;
  display: none;
  align-items: center;
  justify-content: center;
  color: var(--text);
  border: solid 2px;
  border-color: var(--border);
  width: 50px;
  height: 50px;
  border-radius: 50%;
  cursor: pointer;
  font-family: "Helvetica Neue", "Helvetica", "Arial", sans-serif;
  font-size: 2rem;
  text-decoration: none;
  margin-left: 1.5rem;
  margin-right: 1rem;
}

.switch:hover {
  border: 3px solid;
  color: var(--p);
  border-color: var(--p);
}
</style>