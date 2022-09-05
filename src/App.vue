<template>
  <div id="app">
    <MyHeader />
    <MyJumbotron />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader';
import MyJumbotron from './components/MyJumbotron';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbotron
}
}
</script>

<style lang="scss">
@import '@/styles/general.scss';
@import '~@fortawesome/fontawesome-free/css/all.css';
#app {
  height: 100vh;
}
</style>
