<template>
  <div>
    <TheHeader @sidenavToggle="displaySidenav = !displaySidenav" />
    <TheSidenav
      :show="displaySidenav"
      @close="displaySidenav = false"
     />
    <Nuxt />
  </div>
</template>
<script>
import TheHeader from '@/components/Navigation/TheHeader'
import TheSidenav from '@/components/Navigation/TheSidenav'
// import TheHeader from '@/components/Navigation/TheHeader'
export default {
  components: {
    TheHeader,
    TheSidenav
  },
  data() {
    return {
      displaySidenav: false
    }
  }
}
</script>

<style>
  html {
    font-family: Kanit;
  }
</style>
