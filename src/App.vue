<template>
  <the-header title="RememberMe"></the-header>
  <stored-resources :zdroje="storedResources"></stored-resources>
</template>

<script>
import StoredResources from './components/StoredResources.vue';
import TheHeader from './components/layouts/TheHeader.vue';

export default {
  name: 'App',
  components: { StoredResources, TheHeader },
  data() {
    return {
      storedResources: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official Vue.js documentation',
          link: 'https://vuejs.org',
        },
        {
          id: 'google',
          title: 'Google',
          description: ' Uč sa s Googlom',
          link: 'https://google.org',
        },
      ],
    };
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
