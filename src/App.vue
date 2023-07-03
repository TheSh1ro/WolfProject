<script setup>
import { RouterView } from 'vue-router'
import PageHeader from './components/PageHeader.vue'
</script>

<template>
  <PageHeader />
  <RouterView />
</template>

<style>
:root {
  --purple: #c869ff;
  --blue: #83b5ff;
}
* {
  list-style-type: none;
  padding: 0px;
  margin: 0px;
  text-decoration: inherit;
  color: inherit;
  color: inherit;
}
body::-webkit-scrollbar {
  width: 0;
}
#app {
  display: flex;
  flex-direction: column;
}
</style>
