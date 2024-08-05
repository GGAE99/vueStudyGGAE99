<script>
export default {
  props: ['name', 'age', 'isHuman'], // 사용자 정의 속성인 name, age의 값을 받음
  created() {
    console.log('number?' + typeof this.age)
  },
};
</script>
<template>
  <p>이름: {{ name }}</p>
  <p>나이: {{ age }}</p>
  <p>사람임? : {{ isHuman }}</p>
</template>