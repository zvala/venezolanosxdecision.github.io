<template>
  <section>
    <div class="container">
      <h1>Fundación Venezolanos por Decisión</h1>
      <a href=""></a>
    </div>
  </section>
</template>

<style scoped>
section {
  background-image: url("~/static/rsw_1300h_800-12.jpg");
  background-size: cover;
  background-position: center;
  min-height: 100vh;
  text-align: center;
  position: relative;
  isolation: isolate;
  color: #fff;
  display: grid;
  align-items: center;
}

section::after {
  content: "";
  position: absolute;
  background-color: #000;
  opacity: 0.5;
  inset: 0;
  z-index: -1;
}

section div {
  max-width: 1140px;
  margin-inline: auto;
}
</style>
