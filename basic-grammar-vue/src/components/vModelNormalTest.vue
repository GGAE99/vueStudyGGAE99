<script>
export default {
  data() {
    return {
        uid: '',
    };
  },
  methods: {
    login() {
      console.log(`id: ${this.uid}`);
    },
  },
};
</script>
<template>
  <form id="loginForm">
    <label for="uid">아이디: <input type="text" id="uid" v-model="uid" /></label>
    <button type="button" @click="login">로그인</button>
  </form>
</template>