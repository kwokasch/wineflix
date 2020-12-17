<template>
  <section class="secondary-navigation">
    <ul class="navigation-links">
      <UserAvatar
        :url="userAvatar.url"
        :letter="userAvatar.letter"
      />
    </ul>
  </section>
</template>

<script>
import UserAvatar from '@/components/UserAvatar.vue';

export default {
  name: 'SecondaryNavigation',
  components: {
    UserAvatar,
  },
  props: {
    userAvatar: Object,
  },
};
</script>

<style>

</style>
