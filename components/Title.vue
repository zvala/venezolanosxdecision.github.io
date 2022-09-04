<template>
  <h1>
    <slot></slot>
  </h1>
</template>

<script>
export default {
  name: "title",
  props: ["text"],
};
</script>

<style scoped>
h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: "Open Sans", sans-serif;
}

h1 {
  font-size: 72px;
}
</style>
