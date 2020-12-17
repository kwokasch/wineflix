<template>
  <header class="hero">
    <HeroImage />
    <Navigation
      :navigationLinks="navigationLinks"
      :userAvatar="userAvatar"
    />
    <HeroContent
      :title="heroContent.title"
      :subtitle="heroContent.subtitle"
      :imageUrl="heroContent.imageUrl"
      :description="heroContent.description"
    />
  </header>
</template>

<script>
import HeroImage from '@/components/HeroImage.vue';
import Navigation from '@/components/Navigation.vue';
import HeroContent from '@/components/HeroContent.vue';

export default {
  name: 'Hero',
  components: {
    HeroImage,
    Navigation,
    HeroContent,
  },
  props: {
    heroContent: Object,
  },
  computed: {
    navigationLinks() {
      return [{
        label: 'Home',
        url: '#',
        isActive: true,
      }, {
        label: 'Whites',
        url: '#',
        isActive: false,
      }, {
        label: 'Reds',
        url: '#',
        isActive: false,
      }, {
        label: 'Blends',
        url: '#',
        isActive: false,
      }];
    },
    userAvatar() {
      return {
        url: '#',
        letter: 'S',
      };
    },
  },
};
</script>

<style lang="scss">
.hero {
  position: relative;
  color: #fff;
  overflow-y: hidden;
  nav, .hero-content {
    padding: 18px 48px;
  }
}
</style>
