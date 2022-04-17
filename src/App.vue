<template>
  <NavbarComp />
  <NewComp />
  <StatusComp />
</template>

<script>
import NavbarComp from './components/Navbar-Comp.vue'
import NewComp from './components/New-Comp.vue'
import StatusComp from './components/Status-Comp.vue'

export default {
  name: "App",
  components: {
    NavbarComp,
    NewComp,
    StatusComp,
  }
}
</script>

<style>

</style>