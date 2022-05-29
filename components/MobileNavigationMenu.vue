<template>
  <div class="mobile-nav-menu">
    <nuxt-link to="/" v-on:click.native="closeMobileNav" class="mobile-nav-item">Home</nuxt-link>
    <nuxt-link to="/contact" v-on:click.native="closeMobileNav" class="mobile-nav-item">Contact</nuxt-link>
  </div>
</template>

<script>
import { mapMutations } from 'vuex'

export default {
  name: 'MobileNavigationMenu',
  methods: {
    ...mapMutations(['closeMobileNav'])
  }
}
</script>

<style>
.mobile-nav-item {
  font-size: 22px;
  font-weight: 600;
  padding: 20px;
  color: #000000;
  border-bottom: 2px solid #1E2025;
  background-color: #a8e4f5;
}

.mobile-nav-menu {
  display: flex;
  flex-direction: column;
  height: 100vh;
  z-index: 999;
  background-image: url('/beach-wallpaper.jpg');
}
</style>