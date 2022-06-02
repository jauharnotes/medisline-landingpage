<template>
  <div class="flex justify-around items-center gap-20">
    <img src="../../assets/images/logo-medisline-white.svg" alt="logo medisline white" />
    <Splide class="max-w-2xl space-x-4 hidden lg:block" :options="{
      type: 'loop',
      pagination: false,
      drag: 'free',
      focus: 'center',
      perPage: 5,
      autoplay: true,
    }" aria-label="My Favorite Images">
      <SplideSlide>
        <div class="flex-col gap-2 w-24 h-24 border border-white rounded-3xl flex justify-center items-center">
          <img src="../../assets/icons/teleskop-icon.svg" alt="teleskop icon" />
          <p class="text-white font-bold">Umum</p>
        </div>
      </SplideSlide>
      <SplideSlide>
        <div class="flex-col gap-2 w-24 h-24 border border-white rounded-3xl flex justify-center items-center">
          <img src="../../assets/icons/tooth-icon.svg" alt="tooth icon" />
          <p class="text-white font-bold">gigi</p>
        </div>
      </SplideSlide>
      <SplideSlide>
        <div class="flex-col gap-2 w-24 h-24 border border-white rounded-3xl flex justify-center items-center">
          <img src="../../assets/icons/eye-icon.svg" alt="eye icon" />
          <p class="text-white font-bold">mata</p>
        </div>
      </SplideSlide>
      <SplideSlide>
        <div class="flex-col gap-2 w-24 h-24 border border-white rounded-3xl flex justify-center items-center">
          <img src="../../assets/icons/heart-icon.svg" alt="heart icon" />
          <p class="text-white font-bold">jantung</p>
        </div>
      </SplideSlide>
      <SplideSlide>
        <div class="flex-col gap-2 w-24 h-24 border border-white rounded-3xl flex justify-center items-center">
          <img src="../../assets/icons/ear-icon.svg" alt="ear icon" />
          <p class="text-white font-bold">telinga</p>
        </div>
      </SplideSlide>
    </Splide>
  </div>
</template>

<script>
import { Splide, SplideSlide } from '@splidejs/vue-splide';
import '@splidejs/vue-splide/css';
export default {
  components: { Splide, SplideSlide },
  data() {
    return {

    }
  }
};
</script>

<style>
</style>
