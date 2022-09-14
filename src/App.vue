<template>
  <div id="app">
    <HeaderComponent />
    <MainComponent/>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'
import MainComponent from './components/MainComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
  }
}
</script>

<style lang="scss">
@import './style/GeneralStyle.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;

}
</style>
