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

      </main>

    </div>
</template>

<script>
import HeaderDc from './components/HeaderDc.vue'
import MainContent from './components/MainContent.vue'

export default {
  name: "App", 
  components: {
    HeaderDc,
    MainContent
  }
}
</script>

<style lang="scss">
@import './common/variables';
@import './common/common';


</style>
