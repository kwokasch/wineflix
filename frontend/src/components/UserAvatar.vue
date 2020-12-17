<template>
  <span class="user-avatar">
    <a :href="url">{{ letter }}</a>
  </span>
</template>

<script>
export default {
  name: 'UserAvatar',
  props: {
    url: String,
    letter: String,
  },
};
</script>

<style>

</style>
