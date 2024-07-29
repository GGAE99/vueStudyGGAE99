<script>
import vHtmlTest from './components/vHtmlTest.vue';
import vTextTest from './components/vTextTest.vue';
import vPreTest from './components/vPreTest.vue';
import vBindTest from './components/vBindTest.vue';
import vIfTest from './components/vIfTest.vue';
import vShowTest from './components/vShowTest.vue';
import vForArrayTest from './components/vForArrayTest.vue';
import vForObjectTest from './components/vForObjectTest.vue';
import eventObjectCheck from './components/eventObjectCheck.vue';
import modifierTest from './components/modifierTest.vue';
import reactivitySystem from './components/reactivitySystem.vue';
import vOnceTest from './components/vOnceTest.vue';
import vMemoTest from './components/vMemoTest.vue';

export default {
components: {
  vHtmlTest,
  vTextTest,
  vPreTest,
  vBindTest,
  vIfTest,
  vShowTest,
  vForArrayTest,
  vForObjectTest,
  eventObjectCheck,
  modifierTest,
  reactivitySystem,
  vOnceTest,
  vMemoTest,

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
  <vShowTest/>
  <vForArrayTest/>
  <vForObjectTest/>
  <eventObjectCheck/>
  <modifierTest/>
  <reactivitySystem/>
  <vOnceTest/>
  <vMemoTest/>

</template>
<style></style>