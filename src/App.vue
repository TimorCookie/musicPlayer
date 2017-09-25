<template>
  <div id="app">
    <m-header :text="text"></m-header>
    <tab></tab>
    <keep-alive>
      <router-view></router-view>
    </keep-alive>
  </div>
</template>

<script>
import MHeader from 'components/m-header/m-header'
import Tab from 'components/tab/tab'
export default {
  data() {
    return {
      text: 'Timokie'
    }
  },
  components: {
    MHeader,
    Tab
  }
}
</script>

<style lang="scss">
@import '~common/style/index';
</style>
