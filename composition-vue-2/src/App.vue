<script setup>
import { ref, reactive, computed, provide } from 'vue';

import WatchDeepRef from './components/WatchDeepRef.vue';
import WatchReactive from './components/WatchReactive.vue';
import WatchReactiveCallback from './components/WatchReactiveCallback.vue';
import WatchEffect from './components/WatchEffect.vue';
import DefineEmits from './components/DefineEmits.vue';
import Inject from './components/Inject.vue';

// defineEmits
const count = ref(0);
const state = reactive({
  count: 0,
});
const countIncrement = (num1, num2, num3) => {
  console.log(num1, num2, num3);
  count.value = num1 + num2 + num3;
};
const stateCountInrement = (direct, arr) => {
  console.log(direct);
  console.log(arr);
  state.count = direct + arr[0];
};

// inject
const fruits = reactive(['apples', 'bananas', 'oranges']);
const fruitsTxt = computed(() => `I like ${fruits[0]}`);
provide('fruitsArr', fruits);
provide('fruitsText', fruitsTxt);
provide('userObj', { name: 'sucoding', age: 20 });

</script>
<template>
  <!-- <WatchDeepRef />
  <WatchReactive />
  <WatchReactiveCallback /> -->
  <!-- <WatchEffect></WatchEffect> -->
  <h1>{{ count }}</h1>
  <h1>{{ state.count }}</h1>
  <DefineEmits
    @count-increment="countIncrement"
    @state-count-increment="(arr) => stateCountInrement(50, arr)"
  />
  <Inject/>
</template>
