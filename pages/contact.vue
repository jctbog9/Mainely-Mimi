<template>
  <div>
<!-- Desktop Section -->
    <div class="contact-section is-hidden-touch">
      <div class="checkout-image-container">
        <img class="checkout-image" src="checkout.jpeg">
      </div>
      <div class="contact-info-container">
        <contact-info />
      </div>
    </div>

<!-- Mobile Section -->
    <div class="is-hidden-desktop background-section-mobile">
      <div class="title-container">
        <h1 class="cursive">Contact & Directions</h1>
      </div>
      <div class="outside-CTA">
        <div class="checkout-image-container-mobile">
          <img class="checkout-image" src="checkout.jpeg">
        </div>
        <div class="floating-button-container">
          <a class="floating-button" :href="`tel:${2072169750}`">
            <button class="custom-button">
              <font-awesome-icon icon="phone"/> (207) 216-9750
            </button>
          </a>
        </div>
      </div>
      <div class="contact-section-mobile">
        <div class="store-info-section">
          <contact-info />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ContactInfo from '../components/ContactInfo'

export default {
  components: { ContactInfo }
}
</script>

<style>
.background-section-mobile {
  display: flex;
  flex-direction: column;
  width: 100%;
  overflow: hidden;
  justify-content: space-evenly;
}

.title-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 120px;
  background-color: #a8e4f5;
  font-size: 16px;
  width: 100%;
  margin-bottom: 40px;
}

.contact-section {
  display: flex;
  flex-direction: row;
  width: 100%;
  background-color: #ffffff;
  height: 100vh;
  overflow: hidden;
  padding: 40px;
}

.contact-info-container {
  width: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.contact-section-mobile {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
  background-color: rgba(168, 228, 245, 0.86);
}

.checkout-image-container {
  display: flex;
  width: 50%;
  overflow: hidden;
  align-items: center;
}

.checkout-image {
  width: 100%;
}

.outside-CTA {
  display: flex;
  flex-direction: row;
  justify-content: center;
  height: 520px;
  margin-bottom: 40px;
}

.floating-button-container {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  height: 520px;
}

.floating-button {
  position: relative;
  margin-bottom: 20px;
}

.checkout-image-container-mobile {
  width: 320px;
  overflow: hidden;
  position: absolute;
}


.call-section {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  width: 100%;
  background-color: #d3965e;
  padding: 30px;
  align-items: center;
}

.call-section-mobile {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 40px;
}

.store-rules {
  animation: blinker 1.7s cubic-bezier(.5, 0, 1, 1) infinite alternate;  
}

.pizza-image-container {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
  width: 100%;
  background-color: #ffffff;
}

.pizza-image {
  width: 60%;
  margin-bottom: 40px;
  margin-top: 40px;
}
</style>
