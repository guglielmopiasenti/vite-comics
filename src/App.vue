<script setup>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>

<style>
/* CSS Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Generals */
.container {
  margin: 0 auto;
  width: 1200px;
}

img {
  height: auto;
  max-width: 100%;
}

ul {
  list-style-type: none;
}
</style>
