<script >
import appHeader from './components/appHeader.vue';
import appMain from './components/appMain.vue';
import appFooter from './components/appFooter.vue';
export default {
  data() {
    return { count: 0 }
  },
  components:{
    appHeader,
    appMain,
    appFooter
  }
}
</script>

<template>
<appHeader/>
<appMain/>
<appFooter/>

</template>

<style lang="scss" scoped>
$brand_primary: green;

h1{
  color: $brand_primary;
}
</style>
