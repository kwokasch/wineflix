<template>
  <div class="wine">
    <img :src="imageUrl" :alt="label">
    <span v-if="isNew" class="new-badge">New!</span>
    <div v-if="progress" class="amount-consumed">
      <progress min="0" max="100" :value="progress"></progress>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Wine',
  props: {
    imageUrl: String,
    label: String,
    isNew: Boolean,
    progress: Number,
  },
};
</script>

<style>

</style>
