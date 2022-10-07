<template>
  <li>
    <base-card>
      <header>
        <h2>{{ title }}</h2>
        <base-button mode="flat">Odstraniť</base-button>
      </header>
      <p>{{ description }}</p>
      <nav>
        <a :href="link">View Resource</a>
      </nav>
    </base-card>
  </li>
</template>

<script>
import BaseCard from './UI/BaseCard.vue';
export default {
  components: { BaseCard },
  props: ['title', 'description', 'link'],
};
</script>

<style scoped>
li {
  margin: auto;
  max-width: 40rem;
}

h2 {
  margin-bottom: 5px;
}

p {
  margin: 5px 0;
}

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
