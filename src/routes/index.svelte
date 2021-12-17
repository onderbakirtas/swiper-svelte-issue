<script>
  import { Swiper, SwiperSlide } from "swiper/svelte";
  import 'swiper/css'
</script>

<Swiper class="hi" slidesPerView={2} loop={true}>
  <SwiperSlide>Slide 1</SwiperSlide>
  <SwiperSlide>Slide 2</SwiperSlide>
  <SwiperSlide>Slide 3</SwiperSlide>
  <SwiperSlide>Slide 4</SwiperSlide>
  <SwiperSlide>Slide 5</SwiperSlide>
</Swiper>

<style>
  :global(*) {
    box-sizing: border-box;
  }
  :global(body) {
    margin: 0;
  }
  :global(.hi) {
    height: 100vh;
  }
  :global(.swiper-slide) {
    border: 3px solid red;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 3rem;
  }
</style>
