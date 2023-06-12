<template>
  <TheHeader name="MovieMania" />
  <StoredResources :resources="storedResources" />
</template>
<script>
import TheHeader from './components/layouts/TheHeader.vue';
import StoredResources from './components/movie-resources/StoredResources.vue';

export default {
  components: {
    StoredResources,
    TheHeader,
    TheHeader,
  },

  data() {
    return {
      storedResources: [
        {
          id: 'welcomeqqq',
          name: 'welcomeqqqq 2',
          details: 'welcome to the new movie',
          link: 'http://movie.com',
        },
        {
          id: 'zawelcomeqqq',
          name: 'welcomeqqqq 211',
          details: 'welcome xzc zczcsdto the new movie',
          link: 'http://movie2.com',
        },
      ],
    };
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
