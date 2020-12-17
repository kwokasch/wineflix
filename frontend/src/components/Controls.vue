<template>
  <li>
    <PrimaryAction
      label="Drink"
      icon="play"
    />
  </li>
  <li>
    <SecondaryAction
      label="More Info"
      icon="info-circle"
    />
  </li>
</template>

<script>
import PrimaryAction from '@/components/PrimaryAction.vue';
import SecondaryAction from '@/components/SecondaryAction.vue';

export default {
  name: 'Controls',
  components: {
    PrimaryAction,
    SecondaryAction,
  },
};
</script>

<style>

</style>
