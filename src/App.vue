<script >
import appHeader from './components/appHeader.vue';
export default {
  data() {
  },
  components:{
    appHeader,
  }
}

</script>

<template>
  <appHeader/>
</template>

<style lang="scss" scoped>
$brand_primary: green;

h1{
  color: $brand_primary;
}
</style>
