<script >
  import AppHeader from "./components/AppHeader.vue";
  import AppMain from "./components/AppMain.vue";
  import AppFooter from "./components/AppFooter.vue";

  export default {
  components:{
    AppHeader,
    AppMain,
    AppFooter
  },
  data() {
    return {
      count: 0
    }
  }
}
</script>

<template>
  <AppHeader/>
  <AppMain/>
  <AppFooter/>
</template>

<style lang="scss">
  @use "./style/general.scss";


</style>
