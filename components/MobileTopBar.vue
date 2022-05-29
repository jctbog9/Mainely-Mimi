<template>
  <div class="top-bar">
    <div class="top-bar-left">
      <font-awesome-icon v-if="!showMobileNav" icon="bars" v-on:click="handleShowNav"/>
      <font-awesome-icon v-else icon="times" v-on:click="handleShowNav"/>
    </div>
    <div class="top-bar-right">
      <div class="top-bar-right-content">
        Mainely Mimi
      </div>
    </div>
  </div>
</template>

<script>
import { mapMutations, mapActions, mapState } from 'vuex'

export default {
  name: 'TopBar',
  computed: {
    ...mapState(['showMobileNav'])
  },
  methods: {
    ...mapMutations(['openMobileNav', 'closeMobileNav']),
    ...mapActions(['handleShowNav'])
  }
}
</script>

<style scoped>
.top-bar-content {
  color: #ffffff;
}

.nav-element {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 75px;
  width: 100px;
  font-size: 16px;
  color: #ffffff;
}

.logo {
  padding: 5px;
  margin: 5px;
  height: 65px;
}
.top-bar {
  display: flex;
  height: 75px;
  width: 100%;
  background-color: #12A5BD;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.top-bar-left {
  margin: 20px;
  color: white;
}

.top-bar-right {
  align-items: center;
  margin: auto;
}

.top-bar-right-content {
  margin-right: 40px;
  font-family: cursive;
  font-weight: 800;
  font-size: 28px;
  color: #000000;
}
</style>