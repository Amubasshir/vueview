<template>
  <TheHeader name="MovieMania" />
  <TheRecources />
</template>
<script>
import TheHeader from './components/layouts/TheHeader.vue';
import TheRecources from './components/movie-resources/TheRecources.vue';

export default {
  components: {
    TheHeader,
    TheRecources,
    TheRecources,
  },
};
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>
