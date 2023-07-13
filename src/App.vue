<script >
import appHeader from './components/appHeader.vue';
export default {
  data() {
    return { count: 0 }
  },
  components:{
    appHeader,
  }
}
</script>

<template>
  <appHeader/>
  <div>
  <h1>prova</h1>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style lang="scss" scoped>
$brand_primary: green;

h1{
  color: $brand_primary;
}
</style>
