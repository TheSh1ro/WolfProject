<script setup>
import { RouterLink, RouterView } from 'vue-router'
import PageHeader from './components/PageHeader.vue'
</script>

<template>
  <PageHeader />
  <RouterView />
</template>

<style>
* {
  list-style-type: none;
  padding: 0px;
  margin: 0px;
  text-decoration: inherit;
  color: inherit;
}
#app {
  display: flex;
  flex-direction: column;
}
</style>
