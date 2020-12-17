<template>
  <div class="page-white-background">
    This is the shop page
    <div class="container">
      <div>Fabrics</div>
      <div class="item-section">
        <item-card />
        <item-card />
        <item-card />
        <item-card />
        <item-card />
        <item-card />
        <item-card />
        <item-card />
      </div>
    </div>
    
    <div class="container">
      <div>Yarn</div>
      <div class="item-section">
        <item-card />
        <item-card />
        <item-card />
      </div>
    </div>
    
    <div class="container">
      <div>Kits</div>
      <div class="item-section">
        <item-card />
        <item-card />
        <item-card />
        <item-card />
        <item-card />
      </div>
    </div>
  </div>
</template>

<script>
import ContactInfo from '../components/ContactInfo'
import ItemCard from '../components/ItemCard'

export default {
  components: { ContactInfo, ItemCard }
}
</script>

<style>
.page-white-background {
  width: 100%;
  min-height: 100vh;
  background-color: #ffffff;
}

.item-section {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}
</style>