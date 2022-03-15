<template>
  <div class="top-bar">
    <nuxt-link to="/" class="nav-element">Home</nuxt-link>
    <div class="top-bar-content">
      <nuxt-link to="/" class="logo">
        <div>Mainely</div>
        <div>Mimi</div>
      </nuxt-link>
    </div>
    <nuxt-link to="/shop" class="nav-element">Inventory</nuxt-link>
    <nuxt-link to="/contact" class="nav-element">Contact</nuxt-link>
  </div>
</template>

<script>
export default {
  name: 'TopBar'
}
</script>

<style scoped>
.logo {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
  width: 180px;
  font-family: cursive;
  font-weight: 800;
  font-size: 28px;
  color: #000000;
}

.top-bar-content {
  color: #000000;
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

.nav-element:hover {
  background-color: #22242c;
}

.top-bar {
  display: flex;
  height: 75px;
  width: 100%;
  background-color: #12A5BD;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  opacity: 0.99;
  border-bottom: 5px dotted #0790a5;
}

.top-bar-right {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  color: white;
}
</style>