<script >
import appHeader from './components/appHeader.vue';
import appMain from './components/appMain.vue';
import appFooter from './components/appFooter.vue'
export default {
  data() {
  },
  components:{
    appHeader,
    appMain,
    appFooter
  }
}

</script>

<template>
  <header>
  <appHeader/></header>
  <main>
  <appMain/>
  </main>
  <footer>
    <appFooter/>
  </footer>
</template>

<style lang="scss" scoped>
$brand_primary: green;

h1{
  color: $brand_primary;
}
</style>
