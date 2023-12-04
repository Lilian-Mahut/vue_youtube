<script setup lang="ts">
import NavBarItem from './NavBarItem.vue'
import YoutubeIcon from './icons/IconYoutube.vue'
import BurgerIcon from './icons/IconBurger.vue'
import UserIcon from './icons/IconUser.vue'
</script>

<template>
  <NavBarItem>
    <template #burger>
      <BurgerIcon />
    </template>
    <template #logo>
        <YoutubeIcon />
    </template>
    <template #search>
    </template>
    <template #user>
        <UserIcon />
    </template>
  </NavBarItem>
</template>
