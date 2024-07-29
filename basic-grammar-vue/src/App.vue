<script>
import vHtmlTest from './components/vHtmlTest.vue';
import vTextTest from './components/vTextTest.vue';
import vPreTest from './components/vPreTest.vue';
import vBindTest from './components/vBindTest.vue';
import vIfTest from './components/vIfTest.vue';

export default {
components: {
  vHtmlTest,
  vTextTest,
  vPreTest,
  vBindTest,
  vIfTest
},
  data() {
    return {
      name : "철수",
      age : 19,
    };
  },
};
</script>
<template>
  <p>내 이름은 {{ name }}</p>
  <p>내 나이는 {{ age }}</p>
  <p>{{ name.toUpperCase() }}</p>
  <p> {{ age }}</p>

  <vHtmlTest/>
  <vTextTest/>
  <vPreTest/>
  <vBindTest/>
  <vIfTest/>
</template>
<style></style>