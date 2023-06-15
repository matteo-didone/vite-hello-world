<script>
import AppTitle from './components/AppTitle.vue'
import AppHero from './components/AppHero.vue'

export default {
  name: 'App',
  components: {
    AppTitle,
    AppHero
  },

  methods: {
    getImagePath: function (imageName) {
      return new URL(`../assets/${imageName}`, import.meta.url).href;
    }
  }
}
</script>

<script setup>

</script>

<template>
  <AppTitle msg="La mia prima app con Vite!" />
  <AppHero />
</template>

<style scoped></style>


<template>
  <AppTitle msg="La mia prima app con Vite!" />
  <AppHero />
</template>

<style scoped></style>
