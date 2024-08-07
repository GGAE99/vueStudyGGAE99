<script>
import SecondChild from './components/SecondChild.vue';
import LifeCycleHookTest from './components/LifeCycleHookTest.vue';
import PropsTest from'./components/PropsTest.vue';
import DynamicLayout from './components/DynamicLayout.vue';

export default {
  components: {
    SecondChild,
    LifeCycleHookTest,
    PropsTest,
    DynamicLayout,

  },  
  data() {
    return {
      visible: true,
      name : 'sadasd',
      age : 33,
      dynamicName: 'header',
    };
  },
  methods : {
    ageChange() {
      this.age = 55;
    }
  }
  // beforeCreate() {
  //   console.log("beforeCreate");
  // },
  // created() {
  //   setTimeout(() => {
  //     this.visible = false;
  //   }, 3000);
  //   console.log("created");
  // },
  // beforeMount() {
  //   console.log("beforeMount");
  // },
  // mounted() {
  //   console.log("mounted");
  // },
  // beforeUpdate() {
  //   console.log("beforeUpdate");
  // },
  // updated() {
  //   console.log("updated");
  // },
  // beforeUnmount() {
  //   console.log("beforeUnmount");
  // },
  // unmounted() {
  //   console.log("unmounted");
  // },
}

</script>
<template>
  <FirstChild/>
  <SecondChild/>
  <LifeCycleHookTest v-if="visible"/>
  <PropsTest name="aag" age="3" isHuman="true"/> <!--기본 전달-->
  <PropsTest :name="'aag'" :age="3" :isHuman="true"/> <!--v-bind 전달-->
  <p>name: {{ name }} age {{ age }}</p>
  <button @click="ageChange">ifClick data chage</button>
  <DynamicLayout>
    <template #[dynamicName]>
      <h2>동적 슬롯</h2>
    </template>
  </DynamicLayout>
</template>
<style scoped>
h1,
p {
  color: red !important;
}
</style>
