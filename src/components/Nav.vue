<script>
</script>

<template>
  <div class="topbar">
    <div class="focus">
      <a class="contact" href="#contact">Say Hi!</a>
      <label for="theme-switch" class="switch"><span class="sr">Theme Switch</span><i
          class="ri-moon-clear-line"></i></label>
    </div>
  </div>
  <div class="sidebar">
    <div class="line">
      <h2>Kern <br />Stefan</h2>

      <i class="ri-arrow-down-s-line"></i>
    </div>
  </div>
</template>

<style>
.theme-switch:checked .ri-moon-clear-line {
  display: hidden;
  color: red;
}

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
  height: calc(100% - 80px);
  border-left: solid var(--border) 1px;
}

.sidebar h2 {
  text-decoration: none;
  font-weight: normal;
  font-size: 1rem;
  padding-top: 5px;
  padding-left: 0.5rem;
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
  font-size: 1rem;
  padding-left: 0.2rem;
  color: var(--text);
}

.focus {
  float: right;
  margin: 25px;
  margin-right: 2.5rem;
  display: flex;
}

.contact {
  padding: 8px;
  text-decoration: none;
  line-height: 1rem;
  font-weight: bold;
  font-size: 1rem;
  letter-spacing: 2px;
  text-transform: uppercase;
  text-align: center;
  color: var(--text);
  padding-left: 0.6rem;
  padding-right: 0.6rem;
  border: solid;
  border-color: var(--border);
  border-radius: 5px;
  border-width: var(--borderwidth);
}

.contact:hover {
  border: solid calc(var(--borderwidth) + 1px);
}

.switch {
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--text);
  border: var(--borderwidth) solid;
  border-color: var(--border);
  width: 35px;
  height: 35px;
  border-radius: 50%;
  cursor: pointer;
  font-family: "Helvetica Neue", "Helvetica", "Arial", sans-serif;
  font-size: 1.4rem;
  text-decoration: none;
  margin-left: 1.5rem;
  margin-right: 1rem;
}

.switch:hover {
  color: var(--p);
  border-color: var(--p);
  border: solid calc(var(--borderwidth) + 1px);
}
</style>