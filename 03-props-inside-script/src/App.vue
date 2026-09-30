<script setup>

    import { ref } from 'vue';

    import MainNavigation from './components/MainNavigation.vue';
    import SiteFooter from './components/SiteFooter.vue';
    import SiteContent from './components/SiteContent.vue';
    import InputField from './components/inputField.vue';

    const title = ref('VUE')

    setTimeout(() => {
        title.value = 'REACT'
    }, 3000);

    function logMessage(name) {
        // console.log('Input field changed!', name);
        console.log(name);
    }
</script>

<template>
    <header>
        <MainNavigation :title="title" />
        <!-- <MainNavigation /> -->
    </header> 

    <main>
        <SiteContent />
        <InputField @on-input="logMessage"/>
    </main>


    <footer>
        <!-- sitefooter komponens használata -->
        <SiteFooter />
    </footer>

</template>

<style scoped>
</style>
=======
<script>
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
>>>>>>> 8ef920782e682caecd2481add06ab006a93c57c0
