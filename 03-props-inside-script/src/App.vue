<script setup>
import MainNavigation from './components/MainNavigation.vue'
import SiteContent from './components/SiteContent.vue'
import SiteFooter from './components/SiteFooter.vue'
import inputField from './components/inputField.vue/index.js'
const title = ref('VUE')

setTimeout(() => {
  title.value = 'REACT'
}, 3000)

function handleInputClick() {
  alert('Input field clicked!')
}
</script>

<template>
  <header>
    <MainNavigation title="My Vue App" />
  </header>
  <main>
    <SiteContent />
    <inputField />
  </main>
  <footer>
    <!-- sitefooter komponens használata -->
    <SiteFooter />
  </footer>
</template>

<style scoped></style>
