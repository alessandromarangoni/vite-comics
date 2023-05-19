<script>
import AppHeader from './components/AppHeader.vue';
import AppHero from './components/AppHero.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppHero,
    AppMain,
    AppFooter
  }
}
</script>

<template>
  <div>
    <AppHeader />
  </div>
  <div>
    <AppHero />
  </div>
  <div>
    <AppMain />
  </div>
  <div>
    <AppFooter />
  </div>
</template>

<style scoped></style>