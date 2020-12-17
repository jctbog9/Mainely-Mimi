<template>
  <div>
    <div class="mobile-layout is-hidden-desktop">
      <img class="image" src="working.jpeg">
      <contact-info />
      <mobile-carousel />
    </div>
    <div class="page-content is-hidden-touch">
      <div class="contact-info-section">
        <div class="image">
          <img src="open-sign.jpg">
        </div>
        <contact-info />
      </div>
      <div class="featured-image">
        <carousel />
      </div>
    </div>
  </div>
</template>

<script>
import ContactInfo from '../components/ContactInfo'
import Carousel from '../components/Carousel'
import MobileCarousel from '../components/MobileCarousel'

export default {
  components: { ContactInfo, Carousel, MobileCarousel }
}
</script>

<style>
.image {
  width: 460px;
  margin: 0px 0px 10px 0px;
}

.mobile-layout {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.contact-info-section {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  flex-direction: row;
  padding: 40px 0px 50px 0px;
  overflow: hidden;
  background-color: rgba(241,244,249, 0.85)
}

.page-content {
  width: 100%;
  min-height: 60vh;
}

.featured-image {
  display: flex;
  flex-direction: row;
  justify-content: center;
  overflow: hidden;
  background-color: rgba(255, 255, 255, 0.2);
}

.image-content {
  margin: 50px 0px;
  height: 576px;
  width: 1024px;
  overflow: hidden;
}
</style>
