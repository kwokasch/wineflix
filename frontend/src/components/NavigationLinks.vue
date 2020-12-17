<template>
  <li
    v-for="navigationLink in navigationLinks"
    :key="navigationLink.label"
    :class="{ active: navigationLinks.isActive }"
  >
    <NavigationLink
      :url="navigationLink.url"
      :label="navigationLink.label"
    />
  </li>
</template>

<script>
import NavigationLink from '@/components/NavigationLink.vue';

export default {
  name: 'NavigationLinks',
  props: {
    navigationLinks: Array,
  },
  components: {
    NavigationLink,
  },
};
</script>

<style>

</style>
