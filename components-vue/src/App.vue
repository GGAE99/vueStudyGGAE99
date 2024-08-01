<script>
import SecondChild from './components/SecondChild.vue';
import LifeCycleHookTest from './components/LifeCycleHookTest.vue';

export default {
  components: {
    SecondChild,
    LifeCycleHookTest,

  },  
  data() {
    return {
      visible: true,
    };
  },
  beforeCreate() {
    console.log("beforeCreate");
  },
  created() {
    setTimeout(() => {
      this.visible = false;
    }, 3000);
    console.log("created");
  },
  beforeMount() {
    console.log("beforeMount");
  },
  mounted() {
    console.log("mounted");
  },
  beforeUpdate() {
    console.log("beforeUpdate");
  },
  updated() {
    console.log("updated");
  },
  beforeUnmount() {
    console.log("beforeUnmount");
  },
  unmounted() {
    console.log("unmounted");
  },
}

</script>
<template>
  <FirstChild/>
  <SecondChild/>
  <LifeCycleHookTest v-if="visible"/>
</template>
<style scoped>
h1,
p {
  color: red !important;
}
</style>
