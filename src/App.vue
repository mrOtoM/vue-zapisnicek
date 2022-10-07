<template>
  <the-header title="RememberMe"></the-header>
  <the-resources></the-resources>
</template>

<script>
import TheHeader from './components/layouts/TheHeader.vue';
import TheResources from './components/TheResources.vue';

export default {
  name: 'App',
  components: { TheHeader, TheResources },
  data() {
    return {};
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Rubik:wght@300;400;500;600;700&display=swap');

* {
  text-decoration: none;
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  font-family: 'Rubik', sans-serif;
}
</style>
