<script>
import AppHeader from "./components/AppHeader.vue"
import AppMain from "./components/AppMain.vue"
import AppAside from "./components/AppAside.vue"
import AppFooter from "./components/AppFooter.vue"

export default {
  components: {
    AppHeader,
    AppMain,
    AppAside,
    AppFooter,
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppAside />
  <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables.scss' as *;
@import url('https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@400;600;900&display=swap');
</style>
