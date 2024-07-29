<script>
export default {
    data() {
        return {
            message: '<h1>Hello, Vue JS! v-text</h1>',
        };
    },
};
</script>
<template>
  <div>
    <p>v-text 속성을 사용하지 않고 출력한 message = {{ message }}</p>
    <div v-text="message"></div>
  </div>
</template>
<style></style>