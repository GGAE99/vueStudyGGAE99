<script setup>
import { RouterLink, RouterView } from 'vue-router';
</script>
<template>
  <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/about">About</RouterLink>
  </nav>
  <span>beforeView</span>
  <RouterView />
  <span>afterView</span>
</template>
