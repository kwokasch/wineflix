<template>
  <section class="primary-navigation">
    <h1>WineFlix</h1>
    <ul class="navigation-links">
      <NavigationLinks
        :navigationLinks="navigationLinks"
      />
    </ul>
  </section>
</template>

<script>
import NavigationLinks from '@/components/NavigationLinks.vue';

export default {
  name: 'PrimaryNavigation',
  props: {
    navigationLinks: Array,
  },
  components: {
    NavigationLinks,
  },
};
</script>

<style>

</style>
