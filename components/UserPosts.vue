<template lang="pug">
  .user-posts.flex.justify-between
    .header.flex
      p.all Все записи
      p Записи Ильяса
    img(src="~/assets/search_icon.png", alt="alt")
</template>

<style lang="stylus" scoped>
.user-posts
  font-size 13px
  margin-right 15px !important
  padding 15px 15px 0 15px
  background #fff
  border-radius 4px 4px 0 0
  box-shadow 0 1px 0 0 #d3d9de,0 0 0 1px #e7e8ec
  margin 15px 0 0
  img
    padding-bottom 15px
  .header
    p
      color #656565
      padding-bottom 15px
    .all
      color black
      margin-right 20px
      border-bottom 2px solid #5181b8
</style>
