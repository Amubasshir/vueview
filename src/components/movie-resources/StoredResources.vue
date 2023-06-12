<template>
  <ul>
    <MovieResource
      v-for="res in resources"
      :key="res.id"
      :name="res.name"
      :details="res.details"
      :link="res.link"
    />
  </ul>
</template>
<script>
import MovieResource from './MovieResource.vue';
export default {
  inject: ['resources'],
  components: {
    MovieResource,
  },
};
</script>
<style>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}
</style>
