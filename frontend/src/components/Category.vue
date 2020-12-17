<template>
  <section class="category">
    <h2>{{ heading }}</h2>
    <ul>
      <li v-for="wine in wines" :key="wine.id">
        <Wine
          :label="wine.label"
          :imageUrl="wine.imageUrl"
          :progress="wine.progress"
          :isNew="wine.isNew"
        />
      </li>
    </ul>
  </section>
</template>

<script>
import Wine from '@/components/Wine.vue';

export default {
  name: 'Category',
  components: {
    Wine,
  },
  props: {
    heading: String,
    wines: Array,
  },
};
</script>

<style>

</style>
