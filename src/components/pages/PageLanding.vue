<template>
  <the-card />
  <the-description />
  <hr class="mx-[123px] my-[46px] border-darkBlue">
  <the-doctor />
  <the-testimony />
</template>

<script>
import TheCard from '../app/TheCard.vue'
import TheDescription from '../app/TheDescription.vue'
import TheDoctor from '../app/TheDoctor.vue'
import TheTestimony from '../app/TheTestimony.vue'
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