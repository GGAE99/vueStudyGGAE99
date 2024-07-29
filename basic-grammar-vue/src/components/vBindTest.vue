<script>
export default {
    data() {
        return {
            className: 'red-color',
        };
    },
};
</script>
<template>
  <h1 v-bind:class="className">하이 바인드</h1>
</template>
<style>
.red-color {
    color: red
}
</style>