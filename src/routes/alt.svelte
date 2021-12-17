<script>
  import { onMount } from "svelte";
  import { Swiper } from "swiper";
  import "swiper/css";

  const swiper = (node) => {
    const slider = new Swiper(node, {
      slidesPerView: 3,
      loop: true,
    });
  };
</script>

<div class="alt" use:swiper>
  <div class="swiper-wrapper">
    <div class="swiper-slide">1</div>
    <div class="swiper-slide">2</div>
    <div class="swiper-slide">3</div>
    <div class="swiper-slide">4</div>
  </div>
</div>

<style>
  .alt {
    height: 100vh;
  }

  .swiper-slide {
    border: 3px solid green;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 5rem;
  }
</style>
