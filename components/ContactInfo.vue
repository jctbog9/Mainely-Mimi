<template>
  <div class="CTA-content">
    <nuxt-link to="/" class="logo">
        <div>Mainely</div>
        <div>Mimi</div>
      </nuxt-link>
    <div class="location-info">
      <div>
        <font-awesome-icon icon="map-marker-alt"/> 11 Steeple Way, Wells, ME 04090
      </div>
      <div>
        <font-awesome-icon icon="phone"/> (207) 216-9750
      </div>
      <div><font-awesome-icon icon="snowflake"/> Winter Hours:</div>
      <div>Wednesday 9AM - 3PM</div>
      <div>Thursday 9AM - 3PM</div>
      <div>Friday 9AM - 3PM</div>
      <div>Saturday 9AM - 3PM</div>
      <div>Sunday 10AM - 2PM</div>
    </div>
    <a :href="`tel:${2072169750}`">
      <button class="custom-button">Call Now</button>
    </a>
  </div>
</template>

<script>
export default {
  name: 'ContactInfo'
}
</script>

<style>
.logo {
  display: flex;
  flex-direction: column;
  align-content: center;
  align-items: center;
  width: 100px;
  font-family: cursive;
  font-weight: 800;
  font-size: 22px;
  color: #000000;
}

.CTA-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 300px;
  height: 520px;
  justify-content: space-evenly;
  background-color: #d4d2c1;
  padding: 0px 20px 0px 20px;
  border-radius: 2px;
}

.location-info {
  padding: 20px;
  background-color: #ffffff;
  border-radius: 2px;
}
</style>