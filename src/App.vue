<script >
import appHeader from './components/appHeader.vue';
import appMain from './components/appMain.vue'
export default {
  data() {
  },
  components:{
    appHeader,
    appMain
  }
}

</script>

<template>
  <header>
  <appHeader/></header>
  <main>
  <appMain/>
  </main>
</template>

<style lang="scss" scoped>
$brand_primary: green;

h1{
  color: $brand_primary;
}
</style>
