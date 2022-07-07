<template>
    <div id="app">

      <header>
        <HeaderDc />
      </header>

      <!-- Jumbotron -->
      <TopJumbotron />

      <main>
        <!-- Main Content -->
        <section>
          <SeriesList />
        </section>

        <!-- Main Icons Action -->
        <MainIcons />
      </main>

      <footer>
        <!-- Footer Jumbotron -->
        <div>
          <FooterJumbo />
        </div>

        <!-- Social -->
        <div>
          <FooterSocial />
        </div>

      </footer>

    </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import SeriesList from './components/SeriesList.vue'
import MainIcons from './components/MainIcons.vue'
import FooterJumbo from './components/FooterJumbo.vue'
import FooterSocial from './components/FooterSocial.vue'
import TopJumbotron from './components/TopJumbotron.vue'

export default {
  name: "App", 
  components: {
    HeaderDc,
    SeriesList,
    MainIcons,
    FooterJumbo,
    FooterSocial,
    TopJumbotron
  }
}
</script>

<style lang="scss">
@import './common/variables';
@import './common/common';


</style>
