<template>
  <button :type="type" :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['type', 'mode'],
};
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: transparent;
  border: 1px solid #3a0061;
  color: rgb(247, 10, 10);
  cursor: pointer;
}

button:hover,
button:active {
  background-color: rgb(247, 10, 10);
  border-color: #f9003a;
  color: black;
}

.flat {
  background-color: transparent;
  color: #f9003a;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #fa84a0;
}
</style>
