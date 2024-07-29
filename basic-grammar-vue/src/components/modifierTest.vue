<script>
export default {
  methods: {
    onKeyupHandler() {
        console.log('Enter!');
    },
  },
};
</script>
<template>
<div>   
    <input type="text" @keyup.enter = "onKeyupHandler" />
</div>
</template>