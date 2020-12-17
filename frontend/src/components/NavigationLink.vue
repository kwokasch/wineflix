<template>
    <a
      class="navigation-link active"
      :href="url"
    >
      {{ label }}
    </a>
</template>

<script>
export default {
  name: 'NavigationLink',
  props: {
    url: String,
    label: String,
  },
};
</script>

<style>

</style>
