<template>
  <div class="item-card-container">
    <div class="item-card">
      <img src="/stock.jpeg" class="item-image">
    </div>
    <div>NAME OF COLLECTION</div>
    <div>NAME OF SPECIFIC PRODUCT</div>
    <div>$PRICE$</div>
  </div>
</template>

<script>
export default {
  name: 'ItemCard'
}
</script>

<style>
.item-card-container {
  display: flex;
  flex-direction: column;
  margin: 0px 0px 25px 25px;
  align-items: center;
}

.item-card {
  display: flex;
  align-items: center;
  width: 265px;
  height: 265px;
  overflow: hidden;
}

.item-image {
  width: 265px;
}
</style>