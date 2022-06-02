<script>
import BaseLayout from './components/layout/BaseLayout.vue'
import TheFooter from './components/app/TheFooter.vue'
import TheHeader from './components/app/TheHeader.vue'
import TheNavbar from './components/app/TheNavbar.vue'
import ContentLading from './components/app/ContentLading.vue'
  
export default {
  components: {
    BaseLayout,
    TheNavbar,
    TheHeader,
    TheFooter,
    ContentLading,
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
      <content-lading />
    </template>

    <template #footer>
      <the-footer />
    </template>
  </BaseLayout>
</template>