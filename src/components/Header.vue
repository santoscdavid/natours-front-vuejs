<template>
  <header class="header">Some text...</header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
.header {
  height: 95vh;
  background-image: linear-gradient(
      to right bottom,
      rgba(126, 213, 111, 0.8),
      rgba(40, 180, 133, 0.8)
    ),
    url(../assets/hero.jpg);
  background-size: cover;
  background-position: top;

  clip-path: polygon(0 0, 100% 0, 100% 75vh, 0 100%);
}
</style>
