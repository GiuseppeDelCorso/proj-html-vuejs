<script>
import AppHeader from './components/AppHeader.vue'
import AppMain1 from './components/AppMain1.vue'
import AppMain2 from './components/AppMain2.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  AppHeader,
  AppMain1,
  AppMain2,
  AppFooter,

}
</script>

<template>
  <section>
    <AppHeader />
  </section>
  <section>
    <AppMain1 />
  </section>
  <section>
    <AppMain1 />
  </section>
  <section>
    <AppFooter />
  </section>
</template>

<style scoped></style>
