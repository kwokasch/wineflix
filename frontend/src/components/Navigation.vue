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

<style lang="scss">
nav {
  background-color: hsla(0, 0%, 0%, 0.2);
  font-size: 16px;
  display: flex;
  flex-flow: row nowrap;
  justify-content: space-between;
  .primary-navigation {
    display: flex;
    align-items: center;
    .navigation-links {
      display: inline;
      li {
        display: inline-block;
        margin-right: 18px;
        &.active {
          font-weight: 700;
        }
      }
    }
  }
  .secondary-navigation {
    display: flex;
    align-items: center;
  }
}
</style>
