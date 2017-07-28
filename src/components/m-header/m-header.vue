<template>
  <div class="m-header">
    <div class="icon"></div>
    <h1 class="text">{{text}}</h1>
  </div>
</template>
<script>
export default {
  props: {
    text: {
      type: String,
      required: false,
      default: 'Timokie'
    }
  }
}
</script>
<style lang="scss">
@import '~common/style/variable';
@import '~common/style/mixin';
// @import '~common/style/index.scss';
.m-header{
  position: relative;
  height: 44px;
  text-align: center;
  color: $color-theme;
  font-size: 0;
  .icon{
    display: inline-block;
    vertical-align: top;
    margin-top: 6px;
    width: 30px;
    height: 32px;
    margin-right: 9px;
    @include bg-image('logo');
    background-size: 30px 32px;
  }
  .text{
    display: inline-block;
    vertical-align: top;
    line-height: 44px;
    font-size: $font-size-large;
  }
}
</style>
