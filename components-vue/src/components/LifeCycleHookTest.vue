<script>
export default {
  beforeUnmount() {
    console.log("beforeUnmount");
  },
  unmounted() {
    console.log("unmouted");
  },
};
</script>
<template>
  <h1>Life Cycle Test</h1>
</template>
