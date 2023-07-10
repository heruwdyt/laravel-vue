<template>
  <!-- Hero Section Begin -->
  <section class="hero-section">
    <carousel :autoplay="10000" :wrap-around="true">
    <slide :key="slide">
      <div class="single-hero-items set-bg" style="background-image: url('/img/hero-1.jpg')">
    <div class="container">
      <div class="row banner-info">
        <div class="col-lg-5 text-left">
          <span>Bag,kids</span>
          <h1>Black friday</h1> 
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
            do eiusmod tempor incididunt ut labore et dolore
          </p>
          <a href="#" class="primary-btn">Shop Now</a>
        </div>
      </div>
    </div>
  </div>
    </slide>
    <slide :key="slide">
      <div class="single-hero-items set-bg" style="background-image: url('/img/hero-2.jpg')">
    <div class="container">
      <div class="row banner-info">
        <div class="col-lg-5 text-left">
          <span>Bag,kids</span>
          <h1>Black friday</h1> 
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed
            do eiusmod tempor incididunt ut labore et dolore
          </p>
          <a href="/cart" class="primary-btn">Shop Now</a>
        </div>
      </div>
    </div>
  </div>
    </slide>
    <template #addons>
      <navigation />
      <pagination />
    </template>
  </carousel>

    </section>
    <!-- Hero Section End --> 
</template>

<script>
import 'vue3-carousel/dist/carousel.css'
import { Carousel, Slide, Navigation } from 'vue3-carousel'

export default {
  name: 'HeroShayna',
  components: {
    Carousel,
    Slide,
    Navigation,
  },
}
</script>

  <style>
  .set-bg {
    width: 100%;
    height: 500px;
  }
  
  .banner-info {
    margin-top: 80px;
  }
  </style>