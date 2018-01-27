<template lang="html">
    <div :class="$style.test">
        <h1>{{ title }}</h1>
        <p>abcdef</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            title: "abcd",
        }
    },
}
</script>

<style lang="scss" module>
  .test{
    color: rgb(255, 94, 0);
    h1{
      font-size:40px;
    }
  }
</style>
