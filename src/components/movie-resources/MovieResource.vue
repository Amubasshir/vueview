<template>
  <li>
    <base-card>
      <header>
        <h3>{{ name }}</h3>
        <Base-button mode="flat" @click="deleteResource(id)"
          >Delete</Base-button
        >
      </header>
      <p>{{ details }}</p>
      <nav>
        <a :href="link"> View Movie</a>
      </nav>
    </base-card>
  </li>
</template>
<script>
import BaseButton from '../UI/BaseButton.vue';

export default {
  props: ['id', 'name', 'details', 'link'],
  inject: ['deleteResource'],
  components: { BaseButton },
};
</script>
<style>
li {
  margin: auto;
  max-width: 40rem;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

h3 {
  font-size: 1.25rem;
  margin: 0.5rem 0;
}

p {
  margin: 0.5rem 0;
}

a {
  text-decoration: none;
  color: #2f60c9;
}

a:hover,
a:active {
  color: #44b0d7;
}
</style>
