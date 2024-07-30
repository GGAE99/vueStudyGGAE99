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
import VModelNormalTest from './components/vModelNormalTest.vue';
import VModelTextareaTest from './components/vModelTextareaTest.vue';
import vModelCheckboxTest from './components/vModelCheckboxTest.vue';
import VModleRadioTest from './components/vModleRadioTest.vue';
import VModelSelectTest from './components/vModelSelectTest.vue'
import VModelIMETest from './components/vModelIMETest.vue'

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
  VModelNormalTest,
  VModelTextareaTest,
  vModelCheckboxTest,
  VModleRadioTest,
  VModelSelectTest,
  VModelIMETest,

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
  <VModelNormalTest/>
  <VModelTextarea/>
  <vModelCheckboxTest/>
  <VModleRadioTest/>
  <VModelSelectTest/>
  <VModelIMETest/>

</template>
<style></style>