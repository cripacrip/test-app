<template>
  <div id="app">
    <MainPage />
  </div>
</template>

<script>
import MainPage from './components/MainPage.vue'

export default {
  name: 'App',
  components: {
    MainPage
  }
}
</script>

<style>
* {
  box-sizing: border-box;
}
#app {
  font-family: Arial, sans-serif;
  width: 100%;
  margin-top: 21px;
}
p {
  margin: 0;
}
</style>