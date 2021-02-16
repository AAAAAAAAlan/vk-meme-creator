<template lang="pug">
  .create-post.flex.items-center.justify-between
    img.avatar(src="https://sun1-83.userapi.com/s/v1/if1/kIlCdSOPsuHtjml2ga4qEJiEqOTo999pGteV-MAJMPpb2Mk9yI72jLLgXFGs-y-liXuo8v7X.jpg?size=50x0&quality=96&crop=3,116,742,742&ava=1", alt="alt")
    p Напишите что-нибудь...
    .icons.flex
      img(src="~/assets/photo.svg", alt="alt")
      img(src="~/assets/video.svg", alt="alt")
      img(src="~/assets/music.svg", alt="alt")
    .line
    img.color(src="~/assets/color_button_20.png")
</template>

<script>
export default {
  props: {
    yourUrl: {
      type: String,
      required: true,
    },
  },
}
</script>

<style lang="stylus" scoped>
.create-post
  margin-right 15px !important
  padding 15px
  // width 100%
  background #fff
  border-radius 4px
  box-shadow 0 1px 0 0 #d3d9de,0 0 0 1px #e7e8ec
  margin 15px 0 0
  .avatar
    width 28px
    height 28px
    border-radius 50%
  p
    font-size 13px
    color #878787
    margin-right 200px
  .icons
    img
      padding 0 5px
  .line
    width 1px
    height 15px
    background-color #dce1e6
    margin-right 5px
</style>
