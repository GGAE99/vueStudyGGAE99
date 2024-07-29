<script>
export default {
  data() {
    return {
      user : {
        name: "홍길동",
        age: 24,
        gender: "female",
      }
    };
  },
};
</script>
<template>
  <h1>user 객체 요소 꺼내기</h1>
  <ul>
    <li v-for="(value, key, index) in user" :key="index">
      인덱스: {{ index }}, 키: {{ key }} 값: {{ value }}
    </li>
  </ul>
</template>
