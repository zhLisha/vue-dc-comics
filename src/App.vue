<template>
    <div id="app">

      <header>
        <HeaderDc />
      </header>

      <main>
        <!-- Main Content -->
        <section>
          <MainContent />
        </section>

        <!-- Main Icons Action -->
        <MainIcons />
      </main>

      <footer>
        <!-- Footer Jumbotron -->
        <div>
          <FooterJumbo />
        </div>

      </footer>

    </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainContent from './components/MainContent.vue'
import MainIcons from './components/MainIcons.vue'
import FooterJumbo from './components/FooterJumbo.vue'

export default {
  name: "App", 
  components: {
    HeaderDc,
    MainContent,
    MainIcons,
    FooterJumbo
  }
}
</script>

<style lang="scss">
@import './common/variables';
@import './common/common';


</style>
