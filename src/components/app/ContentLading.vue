<template>
  <the-card />
  <the-description />
  <hr class="mx-[123px] my-[46px] border-darkBlue">
  <the-doctor />
  <the-testimony />
</template>

<script>
import TheCard from './TheCard.vue'
import TheDescription from './TheDescription.vue'
import TheDoctor from './TheDoctor.vue'
import TheTestimony from './TheTestimony.vue'
export default {
  components: { TheCard, TheDescription, TheDoctor, TheTestimony },
  data() {
    return {
    }
  }

}
</script>

<style>
</style>