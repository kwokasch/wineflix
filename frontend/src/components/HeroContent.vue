<template>
  <div class="hero-content">
    <h2>
      <img :alt="title" :src="imageUrl">
    </h2>
    <h3>{{ subtitle }}</h3>
    <p>{{ description }}</p>
    <ul class="controls">
      <Controls />
    </ul>
  </div>
</template>

<script>
import Controls from '@/components/Controls.vue';

export default {
  name: 'HeroContent',
  components: {
    Controls,
  },
  props: {
    title: String,
    subtitle: String,
    imageUrl: String,
    description: String,
  },
};
</script>

<style>

</style>
