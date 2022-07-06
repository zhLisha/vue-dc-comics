<template>
    <div id="app">

      <header>
        <HeaderDc />
      </header>

    </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import HeaderDc from './components/HeaderDc.vue'

export default {
  name: "App", 
  components: {
    HeaderDc
  }
}
</script>

<style lang="scss">
@import './common/variables';
@import './common/common';


</style>
