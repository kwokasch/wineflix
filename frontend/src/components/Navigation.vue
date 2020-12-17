<template>
  <nav class="navigation">
    <PrimaryNavigation :navigationLinks="navigationLinks" />
    <SecondaryNavigation :userAvatar="userAvatar" />
  </nav>
</template>

<script>
import PrimaryNavigation from '@/components/PrimaryNavigation.vue';
import SecondaryNavigation from '@/components/SecondaryNavigation.vue';

export default {
  name: 'Navigation',
  components: {
    PrimaryNavigation,
    SecondaryNavigation,
  },
  props: {
    navigationLinks: Array,
    userAvatar: Object,
  },
};
</script>

<style>

</style>
