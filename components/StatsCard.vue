<template lang="pug">
  .stats-card
    h1 {{ stat.number }}
    p {{ stat.text }}
</template>

<script>
export default {
  props: {
    stat: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style lang="stylus" scoped>
.stats-card
  // width 69px
  text-align center
  h1
    // margin-left 7px
    font-size 19px
    color #2a5885
    margin-bottom 5px
  p
    color #828282
    font-size 13px
    white-space nowrap
</style>
