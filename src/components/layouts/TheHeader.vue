<template>
  <header>
    <h1>
      {{ name }}
    </h1>
  </header>
</template>

<script>
export default {
  props: ['name'],
};
</script>

<style scoped>
header {
  width: 100%;
  height: 5rem;
  background-color: #19877e;
  display: flex;
  justify-content: center;
  align-items: center;
}

header h1 {
  color: white;
  margin: 0;
}
</style>
