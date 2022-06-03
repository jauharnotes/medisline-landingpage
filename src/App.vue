<script>
import BaseLayout from './components/layout/BaseLayout.vue'
import TheFooter from './components/app/TheFooter.vue'
import TheHeader from './components/app/TheHeader.vue'
import TheNavbar from './components/app/TheNavbar.vue'
import PageLanding from './components/pages/PageLanding.vue'
  
export default {
  components: {
    BaseLayout,
    TheNavbar,
    TheHeader,
    TheFooter,
    PageLanding,
  }
}
</script>

<template>
  <BaseLayout>
    <template #navbar>
     <the-navbar />
    </template>

    <template #header>
      <the-header />
    </template>

    <template #content>
      <page-landing />
    </template>

    <template #footer>
      <the-footer />
    </template>
  </BaseLayout>
</template>