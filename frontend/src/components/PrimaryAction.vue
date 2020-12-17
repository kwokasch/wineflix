<template>
  <button class="primary-action">
    <FontAwesomeIcon :icon="icon" />
    <span>{{ label }}</span>
  </button>
</template>

<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

export default {
  name: 'PrimaryAction',
  components: {
    FontAwesomeIcon,
  },
  props: {
    label: String,
    icon: String,
  },
};
</script>

<style>

</style>
