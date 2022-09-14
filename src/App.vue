<template>
  <div id="app">
    <HeaderComponent />
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent.vue'

export default {
  name: 'App',
  components: {
    HeaderComponent,
  }
}
</script>

<style lang="scss">
@import './style/GeneralStyle.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;

}
</style>
