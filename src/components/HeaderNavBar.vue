<script setup lang="ts">
import NavBarItem from './NavBarItem.vue'
import YoutubeIcon from './icons/IconYoutube.vue'
</script>

<template>
  <NavBarItem>
    <template #icon>
      <a href="" target="_blank" rel="">
        <YoutubeIcon />
      </a>
    </template>
  </NavBarItem>
</template>