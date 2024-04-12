<script>
import AppHeader from './components/AppHeader.vue';
import AppProductsList from './components/AppProductsList.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppProductsList,
    AppFooter
  },
  data() {
    return {
      links: [
        {
          text: 'Home',
          active: false
        },
        {
          text: 'Prodotti',
          active: true
        },
        {
          text: 'Chi siamo',
          active: false
        },
        {
          text: 'Contatti',
          active: false
        },
      ],
    };
  }
}
</script>

<template>
  <AppHeader :links="links"></AppHeader>

  <main>
    <AppProductsList></AppProductsList>
  </main>

  <AppFooter></AppFooter>
</template>

<style lang="scss">
@use './style/generic';
</style>