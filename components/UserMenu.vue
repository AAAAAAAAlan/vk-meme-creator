<template lang="pug">
  .user-menu
    .photo
      img(:src="imageUrl")
    .btn.message.flex.items-center.justify-center
      p Написать сообщение
      .vl
      img(src="~/assets/gift_icon.png", alt="alt")
    .btn.friends.flex.items-center.justify-center
      p У вас в друзьях
      img(src="~/assets/contour_arrow.svg", alt="alt")
    .call.flex.items-center.justify-start
      img(src="~/assets/phone.svg" alt="alt")
      p Позвонить
    .actions
    br
</template>

<script>
export default {
  props: {
    imageUrl: {
      type: String,
      required: true,
    },
  },
}
</script>

<style lang="stylus" scoped>
.user-menu
  margin-right 15px !important
  padding 15px
  width fit-content
  background #fff
  border-radius 4px
  box-shadow 0 1px 0 0 #d3d9de,0 0 0 1px #e7e8ec
  margin 15px 0 0
  .photo
    img
      border-radius 4px
  .btn
    margin-top 12px
    font-size 12.5px
    width 200px
    height 30px
    border-radius 4px
  .message
    padding 7px 2px 8px
    background-color #5181b8
    color #fff
    .vl
      width 1px
      height 30px
      background-color #6a98cc
      margin-left 11px
    img
      padding-left 15px
  .friends
    background-color #e5ebf1
    p
      color #55677d
    img
      padding-left 10px
  .call
    color #4a76a8
    margin-top 20px
    margin-left 3px
    width 36px
    font-size 13px
    p
      margin-left 10px
</style>
