<script setup lang="ts">
import { RouterLink } from 'vue-router'
import FootBarItem from './FootBarItem.vue'
</script>

<template>
  <FootBarItem>
    <nav>
      <RouterLink to="/">Home</RouterLink>
      <RouterLink to="/about">About</RouterLink>
    </nav>
  </FootBarItem>
</template>
