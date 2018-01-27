<template lang="html">
<!-- 我们先默认用btnClass类，如果它满足不了我们需求的时候，我们自定义类名cname去覆盖btnClass样式 -->
  <div :class="[btnClass,cname]">
    <slot/>
  </div>
</template>
<script>
export default {
  props: {
    cname: {
      type: String,
      default: ''
    }
  },
  data () {
    return {
      btnClass: 'btn',
    }
  }
}
</script>
<style lang="scss">
@import "../../css/element.scss";
.btn{
  @include btn;
}
</style>
