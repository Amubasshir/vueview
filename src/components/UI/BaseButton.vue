<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>

<script>
export default {
  props: ['mode'],
};
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  background-color: transparent;
  border: 1px solid #3a0061;
  color: rgb(6, 84, 120);
  cursor: pointer;
}

/* button:hover,
button:active {
  background-color: rgba(109, 113, 112, 0.283);
  border-color: #9dc4f1;
  color: black;
} */

.flat {
  background-color: #3d40ecf8;
  color: #0d71b9f8;
  color: white;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #7f55e1;
}
</style>
