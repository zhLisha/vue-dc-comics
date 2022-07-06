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

    </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainContent from './components/MainContent.vue'
import MainIcons from './components/MainIcons.vue'

export default {
  name: "App", 
  components: {
    HeaderDc,
    MainContent,
    MainIcons
  }
}
</script>

<style lang="scss">
@import './common/variables';
@import './common/common';


</style>
