<template>
  <div class="flex-col mx-auto lg:w-[1194px] w-full h-auto  lg:h-[600px] rounded-2xl drop-shadow-md bg-white -mt-16 pb-14">
    <div :class="$style.header">
      <the-carausel />
    </div>
    <div class="flex-col items-center">
      <div class="md:flex flex-wrap justify-center items-center gap-10 px-6">
        <my-product />
      </div>
    </div>
  </div>
</template>

<script>
import TheCarausel from './TheCarausel.vue';
import MyProduct from './MyProduct.vue';
export default {
  components: { TheCarausel, MyProduct },
  data() {
    return {

    }
  }
};
</script>

<style module>
.header {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
  padding: 0 79px;
  width: 100%;
  border-top-left-radius: 16px;
  border-top-right-radius: 16px;
  height: 140px;
  background: linear-gradient(90deg,
      #0a80c5 0.04%,
      #1189cb 25.09%,
      #1e9cd7 56.74%,
      #0075be 86.52%,
      #005b97 99.44%);
}
</style>
